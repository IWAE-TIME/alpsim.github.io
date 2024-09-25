
---
title: DWA-01 Revisiting MC05
math: true
toc: true
weight: 1
---

## Quantum phase transitions in the Bose-Hubbard model

**Attention:** this implementation of the directed worm algorithm is an experimental code and should be used only for the Bose Hubbard model without interactions between neighbors. Otherwise the code may crash or yield incorrect results.

As an example of the dwa QMC code we will study a quantum phase transition in the Bose-Hubbard mode.

## Superfluid density in the Bose Hubbard model

### Preparing and running the simulation from the command line

The parameter file `parm1a` sets up Monte Carlo simulations of the quantum Bose Hubbard model on a square lattice with 4x4 sites for a couple of hopping parameters (t=0.01, 0.02, ..., 0.1) using the dwa code.

    LATTICE="square lattice";
    L=4;
 
    MODEL="boson Hubbard";
    Nmax = 2;
    U    = 1.0;
    mu   = 0.5;
 
    T    = 0.1;
 
    SWEEPS=5000000;
    THERMALIZATION=100000;
    SKIP=500;
 
    MEASURE[Winding Number]=1
 
    { t=0.01; }
    { t=0.02; }
    { t=0.03; }
    { t=0.04; }
    { t=0.05; }
    { t=0.06; }
    { t=0.07; }
    { t=0.08; }
    { t=0.09; }
    { t=0.1;  }
    
Using the standard sequence of commands you can run the simulation using the quantum `dwa` code

    parameter2xml parm1a
    dwa --Tmin 5 --write-xml parm1a.in.xml
    
### Preparing and running the simulation using Python

To set up and run the simulation in Python we use the script `tutorial1a.py`. The first parts of this script imports the required modules and then prepares the input files as a list of Python dictionaries:

    import pyalps

    parms = []
    for t in [0.01, 0.02, 0.03, 0.04, 0.05, 0.06, 0.07, 0.08, 0.09, 0.1]:
    parms.append(
        { 
            'LATTICE'                 : "square lattice", 
            'MODEL'                   : "boson Hubbard",
            'T'                       : 0.1,
            'L'                       : 4 ,
            't'                       : t ,
            'mu'                      : 0.5,
            'U'                       : 1.0 ,
            'Nmax'                    : 2 ,
            'THERMALIZATION'          : 100000,
            'SWEEPS'                  : 2000000,
            'SKIP'                    : 500,
            'MEASURE[Winding Number]' : 1
        }
    )
    
We next convert this into a job file in XML format and run the worm simulation:

    input_file = pyalps.writeInputFiles('parm1a', parms)
    res = pyalps.runApplication('dwa', input_file, Tmin=5, writexml=True)

We now have the same output files as in the command line version.

### Evaluating the simulation and preparing plots using Python

To load the results and prepare plots we load the results from the output files and collect the magntization density as a function of magnetic field from all output files starting with `parm1a`. The script is again in `tutorial1a.py`

    import pyalps
    import matplotlib.pyplot as plt
    import pyalps.plot as aplt

    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm1a'),'Stiffness')
    rhos = pyalps.collectXY(data,x='t',y='Stiffness')

    plt.figure()
    aplt.plot(rhos)
    plt.xlabel('Hopping $t/U$')
    plt.ylabel('Superfluid density $\\rho _s$')
    plt.show()

### Setting up and running the simulation in Vistrails

To run the simulation in Vistrails open the file `dwa-01-bosons.vt` and look at the workflow labeled "L=4". Click on "Execute" to prepare the input file, run the simulation and create the output figure.

## The transition from the Mott insulator to the superfluid

We next want to pin down the location of the phase transition more accurately. For this we simulate a two-dimensional square lattice for various system sizes and look for a crossing of the quantity $\rho_s L$.

### Preparing and running the simulation from the command line

In the parameter file `parm1b` we focus on the region around the critical point for three system sizes L=4,6, and 8:

    LATTICE="square lattice";

    MODEL="boson Hubbard";
    Nmax  =2;
    U    = 1.0;
    mu   = 0.5;

    T    = 0.05;

    SWEEPS=2000000;
    THERMALIZATION=150000;
    SKIP=500;

    { L=4; t=0.01; }
    { L=4; t=0.02; }
    { L=4; t=0.03; }
    { L=4; t=0.04; }
    { L=4; t=0.05; }
    { L=4; t=0.06; }
    { L=4; t=0.07; }
    { L=4; t=0.08; }
    { L=4; t=0.09; }
    { L=4; t=0.1;  }

    { L=6; t=0.01; }
    { L=6; t=0.02; }
    { L=6; t=0.03; }
    { L=6; t=0.04; }
    { L=6; t=0.05; }
    { L=6; t=0.06; }
    { L=6; t=0.07; }
    { L=6; t=0.08; }
    { L=6; t=0.09; }
    { L=6; t=0.1;  }

    { L=8; t=0.01; }
    { L=8; t=0.02; }
    { L=8; t=0.03; }
    { L=8; t=0.04; }
    { L=8; t=0.05; }
    { L=8; t=0.06; }
    { L=8; t=0.07; }
    { L=8; t=0.08; }
    { L=8; t=0.09; }
    { L=8; t=0.1;  }
    
Using the standard sequence of commands you can run the simulation using the quantum dwa code

    parameter2xml parm1b
    dwa --Tmin 5 --write-xml parm1b.in.xml

### Preparing and running the simulation using Python

To set up and run the simulation in Python we use the script `tutorial1b.py`. The first parts of this script imports the required modules and then prepares the input files as a list of Python dictionaries:

    parms = []
    for L in [4,6,8]:
    for t in [0.01, 0.02, 0.03, 0.04, 0.05, 0.06, 0.07, 0.08, 0.09, 0.1]:
        parms.append(
            {
            'LATTICE'                 : "square lattice",
            'MODEL'                   : "boson Hubbard",
            'T'                       : 0.1,
            'L'                       : L ,
            't'                       : t ,
            'mu'                      : 0.5,
            'U'                       : 1.0 ,
            'Nmax'                    : 2 ,
            'THERMALIZATION'          : 100000,
            'SWEEPS'                  : 2000000,
            'SKIP'                    : 500,
            'MEASURE[Winding Number]': 1
            }
        )
        
We next convert this into a job file in XML format and run the worm simulation:

    input_file = pyalps.writeInputFiles('parm1b', parms)
    res = pyalps.runApplication('dwa', input_file, Tmin=5, writexml=True)

We now have the same output files as in the command line version.

### Evaluating the simulation and preparing plots using Python

To load the results and prepare plots we load the results from the output files and collect the magntization density as a function of magnetic field from all output files starting with `parm1b`. The script is again in `tutorial1b.py`

    import pyalps
    import matplotlib.pyplot as plt
    import pyalps.plot as aplt

    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm1b'),'Stiffness')
    rhos = pyalps.collectXY(data,x='t',y='Stiffness',foreach=['L'])

    for rho in rhos:
    rho.y = rho.y * float(rho.props['L'])

    plt.figure()
    aplt.plot(rhos)
    plt.xlabel('Hopping $t/U$')
    plt.ylabel('$\\rho _sL$')
    plt.legend()
    plt.title('Scaling plot for Bose-Hubbard model')
    plt.show()

Note the legend and labels that are nicely set up.

### Setting up and running the simulation in Vistrails

To run the simulation in Vistrails open the file `dwa-01-bosons.vt` and look at the workflow labeled "scaling plot".

## Contributors

- Matthias Troyer
- Ping Nang Ma


