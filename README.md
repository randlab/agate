# agate
A groundwater flow data assimilation benchmark

This repository contains the main data files associated to the two synthetic test cases 'A' and 'B' described in the manuscript "Multi-resolution approach to condition categorical multiple-point realizations to dynamic data with iterative ensemble smoothing" published in Water Resources Research (https://doi.org/10.1029/2019WR025875). Additional information including the code used to generate the figures of the test cases can be found in the following repository: https://github.com/lamd91/mends_testcases.

These files are:
- the categorical training image (TI) and the reference simulated by MPS for each case in the GSLIB file format;
- the synthetic head data [m] for each case. Each column corresponds to the time series at one observation location in the order of the
location numbering shown in Figure 8;
- the synthetic flowrate data [m^3/s] for each case. Each column corresponds to the time series associated to each one the five zones 
defined from the bottom to the top of the western boundary;
- the posterior distribution calculated by the Monte Carlo rejection sampling method. Each column corresponds to one sample from the prior 
distribution of unconditional categorical realizations which has been accepted. Note that each column of values is ordered according to 
the values in a GSLIB file for a grid of dimensions 50 x 500 nodes with the origin in the low left corner.
