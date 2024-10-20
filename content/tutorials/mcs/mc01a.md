
---
title: MC-01a Autocorrelations
math: true
toc: true
weight: 2
---

The first tutorial is an introduction to an important topic in Monte Carlo simulations: autocorrelation time. The input files for this tutorial are available in your ALPS distribution, in a directory called `mc-01-autocorrelations`.

## Local updates

We will start with local updates in an Ising model. We will simulate an Ising model on finite square lattices (L=2, 4, ..., 48) at the critical temperature $T_C=2.269186$ using **local** updates.
This tutorial can be run either on the command line or in Python. We recommend the Python version on your local machine, and the command line version for large simulations on clusters.

## Setting up and running the simulation on the command line 

To set up and run the simulation on the command line you first create a parameter file `parm1a`

    LATTICE="square lattice"
    T=2.269186
    J=1
    THERMALIZATION=10000
    SWEEPS=50000  
    UPDATE="local"
    MODEL="Ising"
    {L=2;}
    {L=4;}
    {L=8;}
    {L=16;}
    {L=32;}
    {L=48;}

In order to run the simulation you first need to convert this parameter file into a job file in XML format by typing

    parameter2xml parm1a

This will generate 6 task files (one for each length L) and a job description file parm1a.in.xml which you can open with an XML browser to check the status of your simulation once you started it. The simulation can be started on a single processor by

    spinmc --Tmin 10 --write-xml parm1a.in.xml

or on multiple processors (in our example 8) using MPI by

    mpirun -np 8 spinmc --mpi  --Tmin 10 --write-xml parm1a.in.xml 

(In the following examples we will refer to the single processor commands only.) By setting the argument --Tmin 10 the scheduler initially checks every 10 seconds if the simulation is finished (the time is then dynamically adapted by the scheduler).
You can restart a simulation which has been halted (e.g. due to pressing Ctrl-C or reaching the CPU time limit) by starting the simulation with the XML output file, e.g.

    spinmc --Tmin 10 --write-xml parm1a.out.xml

The option "--write-xml" tells the simulation to store the results of each simulation also in an XML output file (parm1a.task\[1-5\].out.xml) which you can open from the job description file parm1a.out.xml using your XML browser or alternatively by converting the output to a text file using one of the following commands:

    firefox ./parm1a.out.xml
    convert2text parm1a.out.xml

The results of a single task stored for example in parm1a.task1.out.xml can be displayed by using either of the following commands:

- Linux: `firefox ./parm1a.task1.out.xml`
- MacOS: `open -a safari parm1a.task1.out.xml`
- Windows: `"C:\Program Files\Internet Explorer\iexplore.exe" parm1a.task1.out.xml`
- Text output on Linux or MacOS: `convert2text parm1a.task1.out.xml`

Note though that writing XML files can be very slow if you perform many measurements and it is then better to work just with the binary results in the HDF5 files.
To obtain more detailed information on the simulation runs (e.g. to check the convergence of errors) you can convert the run files of the tasks (parm1a.task\[1-6\].out.run1) into XML files by typing

    convert2xml parm1a.task*.out.run1

which will generate the XML output files parm1a.task\[1-6\].out.run1.xml which you can open using your XML browser or alternatively convert to text using either of the commands you used to view the other XML files before.
Look at all six tasks and observe that for large lattices the errors no longer converge by studying the binning analysis in the files parm1a.task\[1-6\].out.run1.xml . To create plots we recommend to use the Python tools described below.

## Setting up and running the simulation in Python

To set up and run the simulation in Python we use the script `tutorial1a.py`. The first parts of this script imports the required modules and then prepares the input files as a list of Python dictionaries:

    import pyalps
    import matplotlib.pyplot as plt
    import pyalps.plot

    parms = []
    for l in [2,4,8,16,32,48]:
    parms.append(
        {
            'LATTICE'        : "square lattice",
            'T'              : 2.269186,
            'J'              : 1 ,
            'THERMALIZATION' : 10000,
            'SWEEPS'         : 50000,
            'UPDATE'         : "local",
            'MODEL'          : "Ising",
            'L'              : l
        }
    )

To run this, launch your python interpreter:

- on Linux or when compiling from source against the system Python: `alpspython`

and then type the commands.

We next convert this into a job file in XML format and by typing

    input_file = pyalps.writeInputFiles('parm1a',parms)

and then run the simulation:

    pyalps.runApplication('spinmc',input_file,Tmin=5,writexml=True)

The option `writexml=True` tells ALPS to write XML files. `spinmc` is the name of the application, `input_file` is the path to the XML job input file, and Tmin=5 again tells ALPS to check every 5 seconds for completion of the simulation.
We next load the binning analysis for the absolute value of the magnetization from the output files, and turn the list of lists into just a flat list:

    binning = pyalps.loadBinningAnalysis(pyalps.getResultFiles(prefix='parm1a'),'|Magnetization|')
    binning = pyalps.flatten(binning)

To make the plots nicer we give each data set a label specifying the size:

    for dataset in binning:
        dataset.props['label'] = 'L='+str(dataset.props['L'])

And finally we create a plot showing the binning analysis graphically:

    plt.figure()
    plt.xlabel('binning level')
    plt.ylabel('Error of |Magnetization|')
    pyalps.plot.plot(binning)
    plt.legend()
    plt.show()

To make separate plots for each system size we make a loop over all data sets:

    for dataset in binning:
        plt.figure()
        plt.title('Binning analysis for L='+str(dataset.props['L']))
        plt.xlabel('binning level')
        plt.ylabel('Error of |Magnetization|')
        pyalps.plot.plot(dataset)
    
    plt.show()

You can clearly see that the errors do not converge for large system sizes.

## Cluster updates

We next repeat the simulations, but using cluster updates. We want to change three parameters:

| **Name** |  |
| :------- | :------- |
| THERMALIZATION | 1000 |
| SWEEPS | 100000 |
| UPDATE | "cluster" |

To run the simulations please follow the same procedure as above, using either
- On the command line the input file `parm1b`
- In Python the script `tutorial1b.py`

You will get curves looking like the ones below. Now the errors have converged and can be trusted.

(missing picture)


## Questions

- Are the errors converged? (To check this convert the run files as described above.)
- Why do longer autocorrelation times lead to slower error convergence?
- On what system parameters do the autocorrelation times depend on? Check by changing parameters in the input file.
- Can you explain why cluster updates are more efficient than local updates?


## Contributors

- Simon Trebst
- Fabien Alet
- Matthias Troyer
- Synge Todo 
- Emanuel Gull



