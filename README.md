# SP2025-FP01-ocean-waves
Final projects repo for the ocean wave/current vs rising global temps analysis

## Group members:
- Molly Bilhartz
- Chandler Bergstrom 

## Project Summary:
We want to learn more about how ocean currents form and change and how different water temperatures can affect these currents/waves in different parts of the globe, but our project will focus on the area of Oahu, Hawaii. We'd like to see how ocean wave patterns have changed over the years and if increasing global temperatures have a measureable affect on these waves.

## Background Information:
Within this project, we will focus on oceanic surface fluid flow, specifically wave patterns off the coast of Honolulu, Hawaii. We will use characteristics such as velocity, wave height, surface water temp, and high/low tide measurements. Wave patterns have been changing over time due to climate change, and we want to be able to graph the data and compare the graphs from each year. From there, we want to predict future patterns and potential changes. 

## Problem Statement:
What are the significant long-term trends in ocean wave characteristics, such as wave height, period, and direction, over the last two decades off the shores of Oahu? Are there observable patterns that can be used to predict futire trends?

## Data Sets:
- NOAA, specifically their World Ocean Database (WOD)
  WOD allows us to look through their database by filtering out or in characteristics we want in our data (geographical areas or certain characteristics such as temperature
NOAA WOD: https://www.ncei.noaa.gov/access/world-ocean-database-select/dbsearch.html

- USGS also has specific data sets for different areas/variables
  We found one for 'High Wave Hazard Intensity Level in the coastal zone of Sand Island (Oahu), Hawaii'
USGS High Wave: https://data.usgs.gov/datacatalog/data/USGS:3a45056a-75c0-4275-9b08-598f88b80361

- NOAA Global Marine Observations in 10-degree Bins derived from the International Comprehensive Ocean-Atmosphere Data Set (ICOADS)
  Use maps to narrow down where we want to get data from and what years data is available for
(ICOADS): https://www.ncei.noaa.gov/access/search/data-search/global-marine?dataTypes=AIR_TEMP&startDate=1990-01-03T00:00:00&endDate=2010-01-03T23:59:59&pageNum=1&pageSize=10

- Nasa's Earthdata: surface currents 1993-2025, 
- https://podaac.jpl.nasa.gov/dataset/OSCAR_L4_OC_NRT_V2.0

### Types of Data being collected:
- Global air temperatures
- Oahu air temperatures
- Ocean surface temperature 
- Ocean wave velocities
- Depth measurements of ocean waves
- Current/wave movement patterns 
  
## Tools/packages being used:
- Pandas: library for data manipulation and analysis, especially useful for working with structured data (will use for DataFrames) link: https://www.kaggle.com/code/kashnitsky/topic-1-exploratory-data-analysis-with-pandas
- Numpy: library for numerical computing, designed to handle arrays and matrices, and perform efficient numerical operations link: https://numpy.org/doc/2.2/user/absolute_beginners.html
- Matplotlib: plotting library for creating static, interactive, and animated visualizations in Python (used for visual graphs and plots to show data) link: https://matplotlib.org/stable/tutorials/pyplot.html
- Xarray: a library designed for working with multi-dimensional datasets and especially useful for time series data, geospatial data link: https://docs.xarray.dev/en/latest/generated/xarray.DataArray.to_dataframe.html
- Cartopy: a library for cartographic projections and mapping, good for visualizing geographical data like ocean currents or wave pattern

## How we will approach the problem:
- We plan to start by pulling air and ocean surface temperature data from public data sites like NOAA, NASA, USGS that we can analyse then look at differnt types of data for waves in Oahu we can analyse to see if there is a common trend with ocean waves that correlates to rising air temperature trends.

## Expected results:
We expect there is going to be clear changes in the variables that we used, velocity, wave height, high tide/low tide, air temp, water surface temp, changes, we thinks its gonna change, wave oatterns are going to be be affected by global warming in the trends from years 2000-2020. (find data then change)

- References:


