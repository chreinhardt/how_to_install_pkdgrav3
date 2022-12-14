# How to install pkdgrav3 for simulating collisions

This repository provides instructions on which software is used for collision simulations with pkdgrav3 and how to install it.

## Required software
- [ pkdgrav3 ]( https://bitbucket.org/dpotter/pkdgrav3/ ): A high performance N-body treecode for self-gravitating astrophysical simulations (Potter et al. 2018) including hydrodynamics using the Smoothed Particle Hydrodynamics (SPH) method
- All software that is listed in [ How to install Gasoline for simulating collisions ]( https://github.com/chreinhardt/how_to_install_gasoline) (except Gasoline of course)

## Installation

Note that there is a README.ubuntu file in the pkdgrav3 repository which provides instructions for installing all required packages on Ubuntu 22.04.

Go to your code directory (e.g., ``` cd ~/code ```) and make a new directory for pkdgrav with ``` mkdir pkdgrav ```. Then clone the pkdgrav3 repository
```
cd pkdgrav
git clone https://bitbucket.org/dpotter/pkdgrav3.git
```
from github. Change to the branch *develop*
```
cd pkdgrav3
git checkout develop
cd ..
```
to use SPH. Now make another directory 
```
mkdir build
```
and compile the code with
```
cd build
cmake ../pkdgrav3
make -j nthreads
```
where *nthreads* is the number of threads by make. This produces the binary file ``` pkdgrav ``` in the build folder.

*Note:* If you have any problem with those steps check the README files in the folder ``` pkdgrav3 ```.

## Running
Make a folder which contains the pkdgrav3 binary, a tipsy binary file with initial conditions and a parameter file. 
