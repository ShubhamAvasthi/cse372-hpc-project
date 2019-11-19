# cse372-hpc-project

This is my project for CSE-372: Introduction to High Performance Computing taught at IIT (BHU) Varanasi.

## Installations
You need to install an MPI implementation (like OpenMPI), mpi4py for MPI bindings and ipyparallel to run "HPC Fast ALP RLS Implementation.ipynb".
1. To install OpenMPI:
   ```console
   $ sudo apt install openmpi-bin
   ```
1. To install mpi4py:  
   ```console
   $ pip install --upgrade mpi4py
   ```
1. To install ipyparallel:  
   ```console
   $ pip install --upgrade ipyparallel
   ```
All other packages can be simply installed using pip.

## Running the code
This applies only to the notebook "HPC Fast ALP RLS Implementation.ipynb", all other notebooks can be run directly.  
To start an ipcluster controller with x number of engines:
```console
$ ipcluster start -n x --engines=MPIEngineSetLauncher
```
For example, for 4 engines:
```console
$ ipcluster start -n x --engines=MPIEngineSetLauncher
```
After running the above command, the Parallel section of the notebook can be executed.
