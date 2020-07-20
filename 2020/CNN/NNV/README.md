Convolutional Neural Network:
-----------------------------

This folder contains the codes and the results for the 'CNN' sub-category of **VNN-COMP 2020**
and NNV took part in the GGN-Nets only. 

MNIST and CIFAR10 were the networks focused for this sub-category.

General File Structure:
-----------------------
1. The 'results' folder contains all the results for the networks in respective dataset specific(i.e MNIST or CIFAR) folders.
2. 'executeXX.py' (XX being the dataset name) is the main execution file which checks the verification results with a threshold time out.
3. 'run_CNN.sh' is the top level script for running all the tests in this sub-category.

NNV Installation:
-----------------
For the installation of NNV, one can follow thw directions of the link: https://github.com/verivital/nnv/blob/master/README.md
The installation needs to be done once, before performing any of the NNV-tests.

P.S. NNV used gurobi linprog optimization ('glpk' can also be used by mantioning it in the argument of verifyRBN function) and for that gurobi 
installation and licensing is required prior to the testing. For setting gurobi linprog to MATLAB path, this link will be helpful:

https://www.gurobi.com/documentation/9.0/quickstart_mac/matlab_setting_up_grb_for_.html

Execution Process:
------------------
1. `cd` to the MATLAB installation directory.
2. Make sure the script is executable by running `chmod +x <path to run_CNN.sh>/run_CNN.sh`from terminal.
3. Run `<path to run_CNN.sh>/run_CNN.sh`.
4. For the first time, run the following matlab command in the terminal to add the nnv paths:
    `matlab -nodisplay -r "addpath(genpath(<path to 'startup_nnv' file>)); addpath(genpath(<path to 'code' folder inside NNV>)); startup_nnv; savepath;"`
5. The run script also lists the configurable parameters for running the test cases.


For any further queries regarding running the tests, please contact: Neelanjana Pal(neelanjana.pal@vanderbilt.edu)
