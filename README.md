# How to install pkdgrav3 for simulating collisions

This repository provides instructions on which software is used for collision simulations with pkdgrav3 and how to install it.

## Required software
- [ pkdgrav3 ]( https://bitbucket.org/dpotter/pkdgrav3/ ): A high performance N-body treecode for self-gravitating astrophysical simulations (Potter et al. 2018) including hydrodynamics using the Smoothed Particle Hydrodynamics (SPH) method
- All software that is listed in [ How to install Gasoline for simulating collisions ]( https://github.com/chreinhardt/how_to_install_gasoline) (except Gasoline of course)

## Installation

Note that there is a README.ubuntu file in the pkdgrav3 repository which provides instructions for installing all required packages on Ubuntu 22.04.

### Gasoline
Go to the gasoline-ics directory (e.g., ```cd ./code/gasoline-ics```) and type
```
make null
```
to compile the code to run on a single CPU or
```
make pthread
```
to obtain a version that runs on several threads using pthread.

*Note:* Make sure that ```mdl``` and ```GSL``` are installed before compiling the code.

