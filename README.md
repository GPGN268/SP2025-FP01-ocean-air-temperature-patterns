# SP2025-FP01-Ocean-Air-Temperature
# Final Project README - Air and surface Ocean temperature correlation patterns

**Group members:** Chandler Bergstrom (cgbergstrom), Molly Bilhartz (mhbilhartz)
**Date:** April 24th, 2025

## Project Summary:
We want to learn more about how the air can impact the surface of the ocean and see if the tempurature of one correlates or affects the otehr at all. Our focus area for this project will focus on the area of Oahu, Hawaii. We want to focus on how the variables of ocean and air temperature are correlated. Air and water temperatures showed consistent seasonal cycles across all years. We used Jupyter Lab coding to graph water and air temperatures across the years of 206-2024. We visualize, compare, and interpret temperature trends from 2016 to 2024 using time-series, anomaly plots, correlation analyses, and heatmaps.

## Background Information:
Within this project, we will focus on oceanic surface fluid flow, specifically wave patterns off the coast of Honolulu, Hawaii. We will use characteristics such as velocity, wave height, surface water temp, and high/low tide measurements. Wave patterns have been changing over time due to climate change, and we want to be able to graph the data and compare the graphs from each year. From there, we want to predict future patterns and potential changes. 

## Problem Statement:
How do ocean and wave temperatures correlate near certain buoy locations? What anomalies exist, and how do they correlate with climate events such as El Niño?

## To Use This Repository:
1) Clone or download the project files.
2) Place raw .txt buoy data files inside the /data directory.
3) Run the Jupyter notebooks step by step:
- data_cleaning.ipynb
- multi_year_visuals.ipynb
- anomaly_analysis.ipynb

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
- *Did not use*

https://www.seanoe.org/data/00412/52367/
https://www.ndbc.noaa.gov/station_page.php?station=51210
https://www.ndbc.noaa.gov/station_history.php?station=51210
https://www.ndbc.noaa.gov/obs.shtml
![image](https://github.com/user-attachments/assets/6069a871-72bd-4dd4-ac08-acb5cf29bb62)


### Types of Data being collected:
- Oahu air temperatures
- Ocean surface temperature 
- Depth measurements of ocean waves
- Current/wave movement patterns 
  
## Tools/packages being used:
- Pandas `pandas`: library for data manipulation and analysis, especially useful for working with structured data (will use for DataFrames) link: pandas.pydata.org
- Numpy `numpy`: library for numerical computing, designed to handle arrays and matrices, and perform efficient numerical operations link: numpy.org
- Matplotlib `matplotlib`: plotting library for creating static, interactive, and animated visualizations in Python (used for visual graphs and plots to show data) link: matplotlib.org
- Xarray `xarray`: a library designed for working with multi-dimensional datasets and especially useful for time series data, geospatial data link: xarray.dev
- Cartopy `cartopy`: a library for cartographic projections and mapping, good for visualizing geographical data like ocean currents or wave pattern
- Seaborn 'seaborn': a visualization library for statistical graphs link:	seaborn.pydata.org

**Objective**  
The primary goal of this study is to investigate whether ocean and air temperatures are correlated in Oahu, Hawaii over the years of 2016-2024. Specifically, we aim to determine whether those characteristics are correlated to anomaly events or if there are certain outliers. We ai, to visualize long-terms patterns in air and sea surface temperatures, create comparitive temperature plots across multiple years, and identify anomalies and relate them to known climte events.

**Project Methodology** 
- Data Collection: Downloaded multi-year .txt buoy files and Argo profiles.
- Data Cleaning: Parsed dates, handled missing values (999.0, <NA>), combined years into unified DataFrames.
- Visualization:
- Yearly comparison graphs (air vs. water temp)
- Anomaly detection plots (monthly vs. baseline)
- Heatmaps showing time vs. temp patterns
- Depth Integration: Argo gridded data used to examine temperature changes below the surface.
- Event Overlay: El Niño years highlighted for anomaly correlation.

**Data Collection**  
- Temperature Data:
Surface air temperature and sea surface temperature data from years 2005-2025 will be pulled from publicly accessible sources such as the **National Oceanic and Atmospheric Administration (NOAA)**, the **National Aeronautics and Space Administration (NASA)**, the **U.S. Geological Survey (USGS)**, the **Argo Global Data Assembly Centers (GDACs)**, and **Scripps Instituiton of Oceanography**.
   
- Wave Height Data
Next, we will collect wave data specific to **Oahu**, focusing on **significant wave height**, a standard metric representing the average height of the highest 1/3 of waves observed over a given period. Data will be pulled from NOAA's **National Data Buoy Center (NDBC)**. 

**Time Period and Seasonal Focus**  
   To isolate seasonal patterns, we will use data from the peak summer months (May–August) and peak winter months (November–February) for each year from 2005-2025. This will allow us to compare long term trends across both high-wave seasons (winter) & low-wave seasons (summer).
   
**Data Processing**  
   All datasets will be processed using **Python** tools to complete the following:
   - Remove missing or negate unneccessary values including unneeded months
   - Align seasonal averages
   - Standardizing units across all datasets
   - Align wave and temperature data as close as possible to Oahu 
   - Ensure all data sets are in the same demensions or merge the data sets using xarray tricks

**Statistical Analysis**
    Structure the data for analysis
   - Isolate long-term trends in air temperature, sea surface temperature, and wave height
   - Analysis visually and mathematically to assess a possible correlation/causation relationship between temperature variables and wave heights in both winter/summer seasons

## Expected results:
- Undeniable correlation between air and sea surface temperature
- Certain years warmer or cooler than others
- Overall warming trend
  
**Hypothesis**  
Based on our current understanding of ocean-atmosphere interactions, we hypothesize that **sea surface and air temperatures in Oahu are closely related and there will be months or years that are warmer than others that may have to do with climate anomalies**, particularly during the summer months when sea surface temperatures are highest. We expect to be able to find evidence that these thermal changes have influenced wave-generating wind patterns and overall ocean dynamics forming larger than 'normal' waves.

**Summary of Results:**
- Air and water temperatures showed consistent seasonal cycles across all years.
- 2023–2024 had clear temperature anomalies consistent with El Niño effects.
- Rolling averages and anomaly plots revealed warming trends, particularly in surface waters.
- Heatmaps and time-depth plots demonstrated thermocline behavior and surface stratification.

**Anticipated Challenges**  
Several challenges may arise in the course of this project:
- **Data availability and resolution**: Long-term and continuous datasets with adequate temporal and spatial resolution may not be available for all the variables we need and/or difficult to find.
- **Data integration**: Merging datasets from different sources may provide issues with formatting, time alignment, variable definitions & dimensioning the sets.
- **Seasonal vs long-term variability**: Distinguishing between short-term variability and long-term trends in our datasets will require very careful indexing during analysis.
- **Causation vs correlation**: Identifying a clear link between rising temperatures and wave changes may be difficult, maybe even impossible, especially when influenced by multiple interacting factors.

**Contribution**
Name | Role
Chandler Bergstrom | Multi-year graphing, data cleaning, heatmap & anomaly development, presentation slides, README updates, Jupyter Lab notebook, and standard deviation and mean graphs
Molly Bilhartz | Gathered Data, README/report formatting

**Code for the graph of station location sites**
import pandas as pd
import matplotlib.pyplot as plt
import cartopy.crs as ccrs
import cartopy.feature as cfeature

path_ds = '../../../../Downloads/30_-160_20_-150.csv'
df = pd.read_csv(path_ds)
df.set_index('STATION', inplace= True)

#Drop rows with missing latitude or longitude
df = df.dropna(subset=['LATITUDE', 'LONGITUDE'])

fig = plt.figure(figsize=(12, 8))
ax = plt.axes(projection=ccrs.PlateCarree())

ax.add_feature(cfeature.COASTLINE)
ax.add_feature(cfeature.BORDERS, linestyle=':')
ax.add_feature(cfeature.LAND, edgecolor='black')
ax.add_feature(cfeature.OCEAN)
ax.add_feature(cfeature.LAKES, alpha=0.5)
ax.add_feature(cfeature.RIVERS)

#ax.set_extent([-160, -150, 18, 32], crs=ccrs.PlateCarree())
ax.set_extent([-161, -149, 18, 32], crs=ccrs.PlateCarree())


ax.scatter(df['LONGITUDE'], df['LATITUDE'],
           color='red', s=10, edgecolor='k',
           transform=ccrs.PlateCarree(),
           label='Station Location - December 2005')

plt.title("Station Locations from Dataset- Hawaii USA", fontsize=15)
plt.legend()
plt.show()
