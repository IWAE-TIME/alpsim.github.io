
---
title: MC-01b Equilibration
math: true
toc: true
weight: 3
---

**Rule of thumb: All Monte Carlo simulations have to be equilibrated before taking measurements.**

## Example: Classical Monte Carlo (local updates) simulations

As an example, we will implement a classical Monte Carlo simulation implemented in the Ising model on a finite square lattice of size $48^2$.

### Preparing and running the simulation from the command line

The parameter file <a href="../codes/mc-01b-equilibration-and-convergence/parm1a" download>`parm1a`</a>:

    LATTICE="square lattice"
    T=2.269186
    J=1
    THERMALIZATION=10000
    SWEEPS=50000  
    UPDATE="local"
    MODEL="Ising"
    {L=48;}

We first convert the input parameters to XML and then run the application `spinmc`:

    parameter2xml parm1a
    spinmc --Tmin 10 --write-xml parm1a.in.xml

### Preparing and running the simulation using Python

The following describes what is going on within the script file <a href="../codes/mc-01b-equilibration-and-convergence/tutorial1a.py" download>`tutorial1a.py`</a>.
The headers:

    import pyalps

    parms = [{
    'LATTICE'         : "square lattice",
    'MODEL'           : "Ising",
    'L'               : 48,
    'J'               : 1.,
    'T'               : 2.269186,
    'THERMALIZATION'  : 10000,
    'SWEEPS'          : 50000,
    }]

Write into XML input file and run the application `spinmc`:

    input_file = pyalps.writeInputFiles('parm1a',parms)
    pyalps.runApplication('spinmc', input_file, Tmin=10, writexml=True)

### Evaluating the simulation and preparing plots using Python

The header:

    import pyalps;

We first get the list of all result files via:

    files = pyalps.getResultFiles(prefix='parm1a')

and then extract, say the timeseries of the |Magnetization| measurements:

    ts_M = pyalps.loadTimeSeries(files[0], '|Magnetization|');
    
We can then visualize graphically:

    import matplotlib.pyplot as plt
    plt.plot(ts_M)
    plt.show()
    
Based on the timeseries, the user will then judge for himself/herself whether the simulation has reached equilibration.

#### A convenient tool: `pyalps.checkSteadyState`

ALPS Python provides a convenient tool to check whether a measurement observable(s) has (have) reached steady state equilibrium. Read here to see how it works.
Here is an example (observable: |Magnetization|) (default: 68.27% confidence interval):

    import pyalps
    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm1a'), '|Magnetization|');
    data = pyalps.checkSteadyState(data);
    
and if you want a 90% confidence interval:

    data = pyalps.checkSteadyState(data, confidenceInterval=0.9);
    
## Convergence

Here, we use the same example in the previous section.

### Using Python

Implementation in Python is straightforward.

    import pyalps
    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm1a'), '|Magnetization|');
    data = pyalps.checkConvergence(data);
    
## Contributors

- Matthias Troyer
- Ping Nang Ma
- Abdullah "Amina" Al-Harbi


