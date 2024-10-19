
---
title: DWA-02 Density Profile
math: true
toc: true
weight: 2
---

## Density profile

As a second example of the dwa QMC code, we will study the density profile of an optical lattice in an harmonic trap.

### Column integrated density

In this subsection, we want to mimick the experimental setup.

#### Preparing and running the simulation from the command line

The parameter file `parm2a` sets up Monte Carlo simulation of a $120^3$ optical lattice trap that mimicks the experiment:

    LATTICE="inhomogeneous simple cubic lattice"
    L=120

    MODEL='boson Hubbard"
    Nmax=20

    t=1.
    U=8.11
    mu="4.05 - (0.0073752*(x-(L-1)/2.)*(x-(L-1)/2.) + 0.0036849*(y-(L-1)/2.)*(y-(L-1)/2.) + 0.0039068155*(z-(L-1)/2.)*(z-(L-1)/2.))"
 
    THERMALIZATION=1500
    SWEEPS=7000
    SKIP=50
 
    MEASURE[Local Density]=1

    { T=1. }
    
Using the standard sequence of commands you can run the simulation using the quantum dwa code

    parameter2xml parm2a
    dwa parm2a.in.xml
    
(This simulation roughly takes 3 hours.)

#### Preparing and running the simulation from Python

To set up and run the simulation in Python we use the script `tutorial2a.py`. The first parts of this script imports the required modules and then prepares the input files as a list of Python dictionaries:

    import pyalps

    parms = [
    {
        'LATTICE' : 'inhomogeneous simple cubic lattice' ,
        'L'       : 120 ,

        'MODEL'   : 'boson Hubbard' ,
        'Nmax'    : 20 ,

        't'  : 1. ,
        'U'  : 8.11 ,
        'mu' : '4.05 - (0.0073752*(x-(L-1)/2.)*(x-(L-1)/2.) + 0.0036849*(y-(L-1)/2.)*(y-(L-1)/2.) + 0.0039068155*(z-(L-1)/2.)*(z-(L-1)/2.))' ,

        'T'  : 1. ,

        'THERMALIZATION' : 1500 ,
        'SWEEPS'         : 7000 ,
        'SKIP'           : 50 , 

        'MEASURE[Local Density]': 1
    }
    ]
    
We next convert this into a job file in XML format and run the worm simulation:

    input_file = pyalps.writeInputFiles('parm2a', parms)
    res = pyalps.runApplication('dwa', input_file)
    
We now have the same output files as in the command line version.
(This simulation roughly takes roughly 3 hours.)

#### Evaluating the simulation and preparing plots using Python

To load the results and prepare the plot for density profile we load the results from the output files from all output files starting with `parm2a`. The script is again in `tutorial2a.py`

    import pyalps
    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm2a'), 'Local Density');

To visualize the column integrated density:

    import pyalps.plot as aplt;
    aplt.plot3D(data, centeredAtOrigin=True)

### Cross section density

We want to observe a Mott plateau.

#### Preparing and running the simulation from the command line

The parameter file `parm2a` sets up Monte Carlo simulation of a $80^3$ optical lattice trap that mimicks the Bloch experiment:

    LATTICE="inhomogeneous simple cubic lattice"
    L=60

    MODEL="boson Hubbard"
    Nmax=20
 
    t=1.
    U=60.
    mu="40. - (0.09416*(x-(L-1)/2.)*(x-(L-1)/2.) + 0.12955*(y-(L-1)/2.)*(y-(L-1)/2.) + 0.11496*(z-(L-1)/2.)*(z-(L-1)/2.))"

    THERMALIZATION=1000000
    SWEEPS=3000000
    SKIP=1000

    MEASURE[Local Density]=1

    { T=1. }
    
Using the standard sequence of commands you can run the simulation using the quantum dwa code

    parameter2xml parm2a
    dwa parm2a.in.xml
    
#### Preparing and running the simulation from Python

To set up and run the simulation in Python we use the script `tutorial2b.py`. The first parts of this script imports the required modules and then prepares the input files as a list of Python dictionaries:

    import pyalps

    parms = [
    {
        'LATTICE' : 'inhomogeneous simple cubic lattice' ,
        'L'       : 60 ,

        'MODEL'   : 'boson Hubbard' ,
        'Nmax'    : 20 ,

        't'  : 1. ,
        'U'  : 60. ,
        'mu' : '40. - (0.09416*(x-(L-1)/2.)*(x-(L-1)/2.) + 0.12955*(y-(L-1)/2.)*(y-(L-1)/2.) + 0.11496*(z-(L-1)/2.)*(z-(L-1)/2.))' ,

        'T'  : 1. ,

        'THERMALIZATION' : 1000000 ,
        'SWEEPS'         : 3000000 ,
        'SKIP'           : 1000 , 

        'MEASURE[Local Density]': 1
    }
    ]
    
We next convert this into a job file in XML format and run the worm simulation:

    input_file = pyalps.writeInputFiles('parm2b', parms)
    res = pyalps.runApplication('dwa', input_file)
    
We now have the same output files as in the command line version.

#### Evaluating the simulation and preparing plots using Python

To load the results and prepare the plot for density profile we load the results from the output files from all output files starting with `parm2b`. The script is again in `tutorial2b.py`

    import pyalps
    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm2b'), 'Local Density');
    
To visualize the cross-section density at the center:

    import pyalps.plot as aplt;
    aplt.plot3D(data, centeredAtOrigin=True, layer="center")

## Contributors

- Matthias Troyer
- Ping Nang Ma


