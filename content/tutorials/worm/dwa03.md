
---
title: DWA-03 Time of Flight Images
math: true
toc: true
weight: 3
---

As a third example of the dwa QMC code, we shall study the time-of-flight images of an optical lattice in an harmonic trap.

## Preparing and running the simulation from Python

To set up and run the simulation in Python we use the script `tutorial3a.py`. The first parts of this script imports the required modules and then prepares the input files as a list of Python dictionaries:

    import pyalps
    import pyalps.dwa

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
        'SWEEPS'         : 60000 ,
        'SKIP'           : 50 , 

        'tof_phase'    : pyalps.dwa.tofPhase(time_of_flight=15.5, wavelength=[765,843,843], mass=86.99) ,

        'MEASURE[Green Function]': 1
    }
    ]
    
We next convert this into a job file in XML format and run the worm simulation:

    input_file = pyalps.writeInputFiles('parm3a', parms)
    res = pyalps.runApplication('dwa', input_file)
    
We now have the same output files as in the command line version.

## Evaluating the simulation and preparing plots using Python

To load the results and prepare the plot for density profile we load the results from the output files from all output files starting with `parm3a`. The script is again in `tutorial3a.py`

    import pyalps
    data = pyalps.loadMeasurements(pyalps.getResultFiles(prefix='parm3a'), 'Green Function');

To visualize the green function:

    import pyalps.plot as aplt;
    aplt.plot3D(data, layer=0)

### The following is rubbish- to be depreciated

    L = pyalps.getParameters(pyalps.input2output(h5_infile))[0]['L'];
    green_tof = pyalps.getMeasurements(pyalps.input2output(h5_infile), observable='Green Function:TOF')[0]['mean']['value'].reshape([L,L,L]);
    momentum_density = numpy.fft.fftn(green_tof).real; 

    V0   = numpy.array([8.805, 8. ,  8. ]);
    wlen = numpy.array([765., 843., 843.]);
    a    = 101;
    m    = 86.99;

    band = pyalps.dwa.bandstructure(V0, wlen, a, m, L);

    q_z   = numpy.array(band.q(2));
    wk2_z = numpy.array(band.wk2(2));

    wk2_z = numpy.array([q_z, wk2_z]).transpose();
    wk2_z0= wk2_z[wk2_z[:,0] == 0.][0][1];
    wk2_z = numpy.transpose(wk2_z[wk2_z[:,1]/wk2_z0 > 1e-4]);
    q_z   = wk2_z[0]
    wk2_z = wk2_z[1]

    momentum_density = numpy.tile(momentum_density, reps=(1,1,2*((q_z[q_z[:] >= 0].size / L)+1)));

    dummy = numpy.zeros(momentum_density.shape[2]);
    dummy[dummy.size/2:dummy.size/2 + q_z[q_z[:] >= 0].size] = wk2_z[q_z[:] >= 0]
    dummy[dummy.size/2-q_z[q_z[:] < 0].size:dummy.size/2]  = wk2_z[q_z[:] < 0]    

    momentum_density = numpy.tensordot(momentum_density, dummy, axes=([2],[0]))
    momentum_density = numpy.tile(momentum_density, reps=(4,4));

    q_x   = numpy.array(band.q(0));
    wk2_x = numpy.array(band.wk2(0));
    wk2_x = wk2_x[(q_x[:] >= -2.)*(q_x[:] < 2.)];
    q_x   = q_x[(q_x[:] >= -2.)*(q_x[:] < 2.)]

    q_y   = numpy.array(band.q(1));
    wk2_y = numpy.array(band.wk2(1));
    wk2_y = wk2_y[(q_y[:] >= -2.)*(q_y[:] < 2.)];
    q_y   = q_y[(q_y[:] >= -2.)*(q_y[:] < 2.)]
 
    wk2 = numpy.outer(wk2_x, wk2_y);

    q_x = numpy.array([q_x] * wk2.shape[1], float);
    q_y = numpy.array([q_y] * wk2.shape[0], float).transpose();
    tof_image = wk2 * momentum_density;


Coarse the grid...
    
    mag = 16;
    q_x = q_x[0:q_x.shape[0]:mag, 0:q_x.shape[1]:mag];
    q_y = q_y[0:q_y.shape[0]:mag, 0:q_y.shape[1]:mag];
    tof_image = tof_image[1:tof_image.shape[0]:mag, 0:tof_image.shape[1]:mag] * mag * mag
    tof_image[tof_image < 0] = 0
