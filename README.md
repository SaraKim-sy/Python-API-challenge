# Python-API-challenge

# Matplotlib-challenge - Pymaceuticals Inc.

## Table of contents
  * [Introduction](#introduction)
  * [Observable Trends based on the Data](#observable-trends)
  * [API keys](#api-keys)
  * [Analysis Report](#final-report)
    * [Scatter Plots](#scatter-plots)
    * [Linear Regression](#linear-regression)
  * [Technologies](#technologies)

## <a name="introduction"></a> Introduction
This project is to create a python script to visualize the weather of 500+ cities across the world of varying distance from the equator utilizing Python libraries such as Pandas, Matplotlib and Citypy, Jupyter Notebook, and the OpenWeatherMap API. In this repository, you will find all of the figures needed for the weather analysis.

* The objective is to build a series of scatter plots to showcase the following relationships:
  * Temperature (F) vs. Latitude
  * Humidity (%) vs. Latitude
  * Cloudiness (%) vs. Latitude
  * Wind Speed (mph) vs. Latitude

* The final notebook will:
  * Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
  * Perform a weather check on each of the cities using a series of successive API calls.
  * Include a print log of each city as it's being processed with the city number and city name.
  * Save both a CSV of all data retrieved and png images for each scatter plot.

* Inside a WeatherPy folder, you will find the following:
  * A jupyter notebook file called [**WeatherPy.ipynb**](./WeatherPy/WeatherPy.ipynb), which is the main script to run for the analysis.
  * A "output_data" folder that contains the analysis output data such as 'cities.csv' and all the plots created.

## <a name="observable-trends"></a> Observable Trends based on the Data
* The Latitude vs. Temperature scatter plot shows that cities that are closer to the equator are high max temperatures. Also, one noticeable thing is that max temperatures of cities in the southern hemisphere roughly range between 40 °F and  110 °F, whereas max temperatures of cities in the northern hemisphere varied in the range of -10 °F and 100 °F. In other words, there are bigger differences between temperatures in the northern hemisphere cities compared to the southern hemisphere cities.
* Looking at the Latitude vs. Humidity scatter plot, it seems that there is no strong correlation between latitude and humidity. 
* The Latitude vs. Cloudiness scatter plot shows that there is no strong correlation between latitude and cloudiness. There are especially many cities with 0%, 40%, slightly under 80%, and 100% cloudiness, respectively, is also noteworthy.
* It seems that there is no strong correlation between latitude and wind speed according to the Latitude vs. Wind Speed scatter plot. Most of the cities have wind speeds in the range of 0 mph and 20 mph. Some cities in the northern hemisphere have relatively higher wind speeds compared to cities in the southern hemisphere. 
* Observable trends based on linear regression are the following:
    * There is a strong negative correlation between temperature and latitude for the cities in the northern hemisphere. The fact that the correlation coefficient was about -0.86 also shows this relationship.
    * There is a moderate positive correlation between temperature and latitude for the cities in the southern hemisphere. The fact that the correlation coefficient was about 0.68 also shows this relationship.
    * There is a weak positive correlation between humidity and latitude for the cities in the northern hemisphere. The fact that the correlation coefficient was about 0.33 also shows this relationship. 
    * There seems to be no correlation between humidity and latitude for the cities in the southern hemisphere. The correlation coefficient was about 0.01. 
    * There seems to be a very weak correlation or no significant correlation between cloudiness and latitude, and wind speed and latitude. 

## <a name="api-keys"></a> API Keys

## <a name="final-report"></a> Analysis Report
The notebook displays the whole analysis is available in this link: [Analysis Report](https://nbviewer.jupyter.org/https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/.ipynb_checkpoints/WeatherPy-checkpoint.ipynb)

### <a name="scatter-plots"></a> Scatter Plots
Scatter Plots created with titles, axis labels, and saved as png files in the "output_data" folder.
* Temperature (F) vs. Latitude

![Lat_vs_Temp](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/lat_vs_temp.png)

* Humidity (%) vs. Latitude

![Lat_vs_Humidity](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/lat_vs_humidity.png)

* Cloudiness (%) vs. Latitude

![Lat_vs_Cloudiness](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/lat_vs_cloudiness.png)

* Wind Speed (mph) vs. Latitude

![Lat_vs_Windspeed](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/lat_vs_windspeed.png)

### <a name="linear-regression"></a> Linear Regression

* Northern Hemisphere - Temperature (F) vs. Latitude

![Northern Temp vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Northern%20Hemisphere-Temperature%20(F)_vs_Latitude-linear_regression.png)

* Southern Hemisphere - Temperature (F) vs. Latitude

![Southern Temp vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Southern%20Hemisphere-Temperature%20(F)_vs_Latitude-linear_regression.png)

* Northern Hemisphere - Humidity (%) vs. Latitude

![Northern Humidity vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Northern%20Hemisphere-Humidity%20(%25)_vs_Latitude-linear_regression.png)

* Southern Hemisphere - Humidity (%) vs. Latitude

![Southern Humidity vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Southern%20Hemisphere-Humidity%20(%25)_vs_Latitude-linear_regression.png)

* Northern Hemisphere - Cloudiness (%) vs. Latitude

![Northern Cloudiness vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Northern%20Hemisphere-Cloudiness%20(%25)_vs_Latitude-linear_regression.png)

* Southern Hemisphere - Cloudiness (%) vs. Latitude

![Southern Cloudiness vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Southern%20Hemisphere-Cloudiness%20(%25)_vs_Latitude-linear_regression.png)

* Northern Hemisphere - Wind Speed (mph) vs. Latitude

![Northern Wind vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Northern%20Hemisphere-Wind%20Speed%20(mph)_vs_Latitude-linear_regression.png)

* Southern Hemisphere - Wind Speed (mph) vs. Latitude

![Southern Wind vs Lat](https://github.com/SaraKim-sy/Python-API-challenge/blob/main/WeatherPy/output_data/Southern%20Hemisphere-Wind%20Speed%20(mph)_vs_Latitude-linear_regression.png)

## <a name="technologies"></a> Technologies
Project is created with:
* Python 3.8
* Jupyter Notebook
* Pandas
* Matplotlib
* OpenWeatherMap API
* Citipy
