# Carbon dioxide as a line active agent
## Description
This repository contains the scripts that are necessary to run the simulations of the article:

*Carbon dioxide as a line active agent: its impact on line tension and nucleation rate*


## Structure of the repository
The repository is divided in two folders corresponding to the simulations on the two different solids. Each folder is divided in subfolders corresponding to the different simulation points. Each subfolder is named according to the number of CO2 molecules that have been simulated.

- `hydrophobic` : simulations on a hydrophobic solid
  - `0`
  - `40`
  - `80`
  - `120`
  - `160`
  - `200`
  - `240`
  - `280`
- `hydrophilic` : simulations on a hydrophilic solid
  - `0`
  - `160`
  - `320`
  - `480`
  - `640`

In each subfolder there are 11 input files that correspond to a short initialization simulation followed by ten simulations of 5ns length each. The simulations shall be launched sequentially because the output of simulation n is the input of simulation n+1. The initial location of atoms is stored in the data.INIT.txt file.  


## LAMMPS version
All simulations have been run using the 17th November 2016 stable release of [LAMMPS](https://github.com/lammps/lammps).


## License
All the scripts of this repository are made available under the open source Apache2.0 license.