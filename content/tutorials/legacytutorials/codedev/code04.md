
---
title: Code-04 Vistrails Package simple
math: true
toc: true
weight: 5
---

In this tutorial we will use our Ising example to illustrate how one can create a Vistrails package. Go to your vistrails userpackages directory:

    cd $HOME/.vistrails/userpackages

and copy the contents of the directory `ising-package` into it. Then add your `python.py` file from the [Code-01 Tutorial](../../codedev/code01).

By doing so we have derived "IsingSimulation" from a Vistrails Module class and specified the input ports for our input parameters as well the output port for our result file. If you now open your Vistrails application, choose "Preferences" from the Menu and go to "Module Packages". You will find a Package called "isingpackage", which you can enable. You can now start incorporating your own Module in a Vistrail! See `simple_package.vt` as an example.

## Some more details

Vistrails packages must contain the two files `__init__.py` and `init.py`. These take care of separate tasks:

- `__init__.py` declares the package (name, identifier, version) and defines dependencies.
- `init.py` should initialize the package. This involves tasks such as registering modules etc.

The reason for this separation is to make the package reloadable. If all of the initialization is placed in `__init__.py`, the package cannot be reloaded after the first instantiation.

### Package declaration

The package needs to be declared in the `__init__.py` file. The declaration contains identifier, version and name, all of which should be strings. A method `package_dependencies()` can return a list of identifiers which specify dependency relations.

    identifier = 'org.comp-phys.ising'
    version = '2.0.0'
    name = 'ALPS Ising tutorial'

    def package_dependencies():
    return []

### Defining modules

We will now go through the definition of the `IsingSimulation` module.

    from core.modules.vistrails_module import Module
    import core.modules.basic_modules
    import ising
    basic = core.modules.basic_modules

These lines import some of the relevant packages from Vistrails. In particular, we import all the basic modules of Vistrails, such as Integer, List, etc., into the namespace basic. These can be used to define input and output ports of our custom module.
All Vistrails modules must, directly or indirectly, be derived from the class Module. In our example, we derive directly from Module:

    class IsingSimulation(Module):
    
Also, all modules must contain
- a method compute(self), which is called on execution of the workflow,
- a definition of input and output ports in the static variables `_input_ports` and `_output_ports`. These should be lists of tuples with the first element being the name of the port and the second element being a list that defines properties of the port, such as types.

Below is the definition of the `compute()` method for our example:

    def compute(self): 
       result_file = self.interpreter.filePool.create_file(suffix='.h5')
       L = self.getInputFromPort('L')
       beta = self.getInputFromPort('beta')
       N = self.getInputFromPort('N')
       sim = ising.Simulation(beta,L)
       sim.run(N/2,N)
       sim.save(result_file.name)
       
       self.setResult('result_file', result_file)  

In our example, the input ports should define the system size L, the inverse temperature beta, and the number of sweeps N. The output is an HDF5 file containing the results of the simulation. In this example, we only set the type of the output port, so that the second element in the tuples is a list of length one containing the name of a Vistrails module.

    _input_ports = [('L', [basic.Integer]),
                    ('beta', [basic.Float]), ('N', [basic.Integer])]
   _output_ports = [('result_file', [basic.File])] 

To access the input and output ports from the module, the `getInputFromPort()` and `setResult()` methods of Module should be used. Note that while the ports have to be declared with a type that has to be a valid Module class, due to weak typing in Python any type can be stored into or read from ports.

### Registering modules

The easiest way to register a module with Vistrails is to add it to a global variable `_modules` in the `init.py` file:

    _modules = [IsingSimulation]
