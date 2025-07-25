## GRL - BAM spatial analysis

This repository includes the results of the spatial discharge changes analysis along the mainstem of the Yellow River, and script to visualize them.
The river discharge was estimated using the [bamr](https://github.com/markwh/bamr) algorithm [Hagemann et al., 2017](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2017WR021626) base on the satellite-derived river width and the prior guess of discharge. The river width was extracted from Landsat TM images by the [RivWidthCloud](https://github.com/seanyx/RivWidthCloudPaper) algorithm ([Yang et al., 2019](https://ieeexplore.ieee.org/document/8752013)) and the prior discharge was given from [GRADES](https://www.reachhydro.org/home/records/grades) ([Lin et al., 2019](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019WR025287)).

### result_figures.ipynb

This code loads the results at **dat** directory, and draws the figures for the manuscript.

### dat
#### reach_results_conventional.csv & reach_results_virtual.csv 

The river discharge estimates by the BAM for the targeted reaches in the two experiments were summarized in these csv file with several ancillary data for analysis.

#### gauge

This sub-directory includes BAM-predicted discharge and the observed discharge on the Landsat data acquisition date for the 19 gauges.
