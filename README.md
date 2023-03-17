# Leveraging Python for Spatial Data Science

[CARTO Spatial Data Science Bootcamps](https://spatial-data-science-conference.com/bootcamps/2023/) | March 23, 2023

Instructor: [Will Geary](https://www.linkedin.com/in/willgeary/), Senior Data Scientist at [Revel Transit](https://gorevel.com/)

In this workshop, we will perform spatial analysis on ridehail trips in NYC. We will cover the following:

    1) Perfom some necessary cleaning on the data
    2) Illustrate the Modifiable Areal Unit Problem (MAUP) and why we shouldn't simply analyze raw count of pickups
    3) Calculate pickup density per zone
    4) Make some simple choropleth maps
    5) Perform a statistical Cluster and Outlier analysis. This requires a few steps:
        a) Create a Spatial Weights matrix
        b) Introduce the concept of spatial autocorrelation
        c) Introduce the Local Moran's I statistic (a local measurement of spatial autocorrelation)
        d) Detect statistically significant clusters (hotspots & coldspots) and outliers (diamonds & doughnuts)
        
See [notebook.ipynb](https://github.com/willgeary/PythonSpatialDataScience/blob/main/notebook.ipynb) for the complete code behind this workshop.

## [Optional] Setup Instructions

This workshop will require Python 3 and several packages, including `geopandas`, `contextily`, `seaborn`, `libpysal`, `esda`, `splot`, and `osmnx`. 

You can simply install the above in your own existing Python enviroment, or if you wish, you may optionally spin up a conda environment to exactly match mine with the following steps.

1) Clone the repository:

`git clone https://github.com/willgeary/PythonSpatialDataScience`

2) Change directory into the respository:

`cd PythonSpatialDataScience`

3) Create the conda environment:

`conda env create --file environment.yml --force`

4) Activate the conda environment:

`conda activate spatialstats`

5) Add the environment as a kernel to Jupyter Lab:

`python -m ipykernel install --sys-prefix --name spatialstats`

6) Launch Jupyter Lab:

`jupyter lab`

Proceed to launch `notebook.ipynb` using the `spatialstats` kernel.
