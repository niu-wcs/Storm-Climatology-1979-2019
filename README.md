# Trends and Variability of North American Extratropical Cyclones: 1979–2019
## Code Release for Publication - J. Apl. Metor. Climo.
### Python 3
### Robert Fritzen, Victoria Lang, Victor Gensini

## Introduction
This code is based off of the eddy tracking algorithm written by Eric Oliver (https://github.com/ecjoliver/stormTracking). This project used the North American Regional Analysis as the input data source to track low-pressure cyclones across North America between 1979 - 2019.

This code has been updated to Python 3, and fixed to adjust segments of code that used depricated Python 2 features or packages that were no longer suitable given the new Python 3 standards.

## Usage
This code can be run with a minimal anaconda-3 installation and a few extra packages installed, they include:
* numpy
* scipy
* matplotlib
* netCDF4

Additional packages are required to use all of the plotting routines and the census module, these are:
* geopandas
* descartes
* cartopy

The **Storm Detection and Tracking** notebook will guide you through the process of running the eddy detection and tracking algorithms on your incoming data source (Currently configured for NARR (mslet)), generating two output files *storm_det_slp* and *storm_track_slp*. These two output files can then be passed to the other two files in the notebook to generate figures and the census block to run repitition tests or comparative analysis, or to be used on additional datasets or in the future for an "update" study.