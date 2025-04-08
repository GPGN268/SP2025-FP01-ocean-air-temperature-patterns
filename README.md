# SP2025-FP01-ocean-waves
# Final Project README - Could Global Warming be disrupting our Ocean Waves and Currents?

**Group members:** Chandler Bergstrom, Molly Bilhartz
**Date:** Molly Bilhartz

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
- Pandas `pandas`: library for data manipulation and analysis, especially useful for working with structured data (will use for DataFrames) link: https://www.kaggle.com/code/kashnitsky/topic-1-exploratory-data-analysis-with-pandas
- Numpy `numpy`: library for numerical computing, designed to handle arrays and matrices, and perform efficient numerical operations link: https://numpy.org/doc/2.2/user/absolute_beginners.html
- Matplotlib `matplotlib`: plotting library for creating static, interactive, and animated visualizations in Python (used for visual graphs and plots to show data) link: https://matplotlib.org/stable/tutorials/pyplot.html
- Xarray `xarray`: a library designed for working with multi-dimensional datasets and especially useful for time series data, geospatial data link: https://docs.xarray.dev/en/latest/generated/xarray.DataArray.to_dataframe.html
- Cartopy `cartopy`: a library for cartographic projections and mapping, good for visualizing geographical data like ocean currents or wave pattern

### How we will approach the problem:
**Study Design and Methodology**

1. **Objective**  
   The primary goal of this study is to investigate whether long-term increases in air and ocean surface temperatures are associated with changes in ocean wave heights in Oahu, Hawaii. Specifically, we aim to determine whether wave heights during peak seasonal months (summer (May, June, July, August) and winter (November, December, January, February)) have increased over a 20 year period. We aim to be able to pin point whether or not wave height trends correlate with warming trends in the atmosphere and ocean.

2. **Data Collection**  
   a) **Temperature Data**  
   Surface air temperature and sea surface temperature data from years 2005-2025 will be pulled from publicly accessible sources such as the **National Oceanic and Atmospheric Administration (NOAA)**, the **National Aeronautics and Space Administration (NASA)**, the **U.S. Geological Survey (USGS)**, the **Argo Global Data Assembly Centers (GDACs)**, and **Scripps Instituiton of Oceanography**. Where possible, we will prioritize datasets that offer high temporal resolution and spatial relevance to the Hawaiian Islands, specifically Oahu, Hawaii.
   
   b) **Wave Height Data**  
   Next, we will acquire historical wave data specific to **Oahu**, focusing on **significant wave height**, a standard metric representing the average height of the highest one-third of waves observed over a given period. Data will be sourced from NOAA's **National Data Buoy Center (NDBC)**. 

3. **Time Period and Seasonal Focus**  
   To assess seasonal patterns, we will isolate data from the **peak summer months (May–August)** and **peak winter months (November–February)** for each year from 2005-2025. This will allow us to compare long-term trends across both **high-wave seasons** (typically winter) and **low-wave seasons** (typically summer).

4. **Data Processing**  
   All datasets will be processed using **Python** tools to complete the following:
   - Remove missing or negate unneccessary values including unneeded months
   - Aligning seasonal average
   - Standardizing units across all datasets for flow in analysis
   - Align wave and temperature data as closely as possible to Oahu
   - Ensure data sets are in the same demensions or merge the data sets using


5. **Statistical Analysis**
    Structure the data for analysis
   - Isolate long-term trends in air temperature, sea surface temperature, and wave height
   - Analysis visually and mathematically to assess a possible correlation/causation relationship between temperature variables and wave heights in both winter/summer seasons

### Expected results:

**Hypothesis**  
Based on our current understanding of ocean-atmosphere interactions, we hypothesize that **rising ocean and air temperatures associated with global climate change are contributing to increased wave energy in Oahu**, particularly during the summer months when sea surface temperatures are highest. We expect to be able to find evidence that these thermal changes have influenced wave-generating wind patterns and overall ocean dynamics forming larger than 'normal' waves.

Specifically, we expect to find:
- An **upward trend** in average wave height during summer months between 2005 and 2025
- An **increased seasonal wave amplitude**, potentially reducing the gap between summer and winter wave heights  
- A possible correlation between higher air/sea surface temperatures and increased wave velocity or intensity

**Expected Results**  
We expect to observe significant changes in the following variables:
- Wave height
- Wave velocity
- High and low tide extremes
- Air temperature
- Sea surface temperature

**Expected Significance**  
Understanding the relationship between warming trends and ocean wave behavior is critical for:
- Coastal erosion modeling and shoreline management
- Infrastructure planning in vulnerable coastal communities
- Surf tourism and recreational safety
- Contributing to broader climate impact assessments in the Pacific region

**Anticipated Challenges**  
Several challenges may arise in the course of this project:
- **Data availability and resolution**: Long-term and continuous datasets with adequate temporal and spatial resolution may not be available for all the variables we need and/or difficult to find.
- **Data integration**: Merging datasets from different sources may present issues with formatting, time alignment, and variable definitions and dimensioning.
- **Seasonal vs long-term variability**: Distinguishing between short-term variability and long-term trends in our datasets will require very careful indexing in the time-series analysis.
- **Causation vs correlation**: Identifying a clear link between rising temperatures and wave changes may be difficult, maybe even impossible, especially when influenced by multiple interacting factors.


