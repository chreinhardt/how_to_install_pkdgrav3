# How to install pkdgrav3 for simulating collisions

This repository provides instructions on which software is used for collision simulations with pkdgrav3 and how to install it.

## Required software
- [ pkdgrav3 ]( https://bitbucket.org/dpotter/pkdgrav3/ ): A high performance N-body treecode for self-gravitating astrophysical simulations (Potter et al. 2018) including hydrodynamics using the Smoothed Particle Hydrodynamics (SPH) method
- All software that is listed in [ How to install Gasoline for simulating collisions ]( https://github.com/chreinhardt/how_to_install_gasoline) (except Gasoline of course)

## Installation

Note that there is a README.ubuntu file in the pkdgrav3 repository which provides instructions for installing all required packages on Ubuntu 22.04.

### pkdgrav

Go to your code directory (e.g., ``` cd ~/code ```) and make a new directory for pkdgrav with ``` mkdir pkdgrav ```. Then change into this directory (``` cd pkdgrav ```) and clone the pkdgrav3 repository
```
git clone https://bitbucket.org/dpotter/pkdgrav3.git
```
from github. Now make another directory (e.g., ``` mkdir build ```) and run ``` cmake ../pkdgrav3 ```.

*Note:* If you have any problem with those steps check the README files in the folder ``` pkdgrav3 ```.

