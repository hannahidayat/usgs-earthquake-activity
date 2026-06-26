[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hannahidayat/usgs-earthquake-activity/HEAD?urlpath=%2Fdoc%2Ftree%2Fearthquakes.ipynb)

Click on the badge above to run this notebook within browser via MyBinder. 

# USGS Earthquake Activity 

## Overview

Real-time seismic data over a 24-hour window from the [U.S. Geological Survey](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) is retrieved to analyze worldwide earthquake activity.   

Tools for analysis and visualization include Pandas, GeoPandas, Matplotlib, and Seaborn. 

## Key Findings

### Analysis & Seismic Classification 
Timestamp data was used to identify the hour with the most seismic activity and to aggregate hourly earthquake counts. 

![Hourly count](https://github.com/hannahidayat/usgs-earthquake-activity/blob/main/images/Screenshot%202026-06-26%20131353.png)


Based on z-coordinate, earthquakes were grouped and counted based on Earth's structural layers: crustal, upper mantle, and deep mantle. 
The z-coordinate (depth) was extracted from `geometry` of the GeoJSON to locate the deepest earthquake event in the past 24 hours. 

![Classification](https://github.com/hannahidayat/usgs-earthquake-activity/blob/main/images/Screenshot%202026-06-26%20132032.png)


### Data Visualization

A global density map was created to visually highlight regions experiencing the highest density of seismic activity. Hexagonal points are used to represent the number of earthquakes in a location. 

![Density map](https://github.com/hannahidayat/usgs-earthquake-activity/blob/main/images/Screenshot%202026-06-26%20110201.png)
*Static images of a single 24-hour cycle. Launch the interactive MyBinder to see updated data.* 

A scatter plot was designed to compare earthquake event intensity and tectonic boundaries through magnitude versus depth profiling. 

![Scatter plot](https://github.com/hannahidayat/usgs-earthquake-activity/blob/main/images/Screenshot%202026-06-26%20112354.png)
