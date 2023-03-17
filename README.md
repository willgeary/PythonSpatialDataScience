# Leveraging Python for Spatial Data Science

[CARTO Spatial Data Science Bootcamps](https://spatial-data-science-conference.com/bootcamps/2023/) | March 23, 2023

Instructor: [Will Geary](https://www.linkedin.com/in/willgeary/), Senior Data Scientist at [Revel Transit](https://gorevel.com/)

In this workshop, we will perform spatial analysis on ridehail trips in NYC. We will cover the following:

    1) Perfom some necessary cleaning on the data
    2) Illustrate the Modifiable Areal Unit Problem (MAUP) and why we can't simply analyze the count of pickups per zone
    3) Calculate pickup density per zone
    4) Make some simple choropleth maps
    5) Perform a statistical Cluster and Outlier analysis. This requires a few steps:
        a) Create a Spatial Weights matrix
        b) Introduce the concept of spatial autocorrelation
        c) Introduce the Local Moran's I statistic (a local measurement of spatial autocorrelation)
        d) Detect statistically significant clusters (hotspots & coldspots) and outliers (diamonds & doughnuts)
        
See [notebook.ipynb](https://github.com/willgeary/PythonSpatialDataScience/blob/main/notebook.ipynb) for the complete code behind this workshop.

## Optional Setup Instructions

This workshop will require Python 3 and several packages, including `geopandas`, `contextily`, `seaborn`, `libpysal`, `esda`, `splot`, and `osmnx`. 

You can simply install the above in your own existing Python enviroment, or if you wish, you may optionally spin up a conda environment called `spatialstats` to exactly match mine with:

`conda env create --file environment.yml --force`

and activate it with:

`conda activate spatialstats`
