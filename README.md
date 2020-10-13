# World Weather Analysis & Visualization

## Summary
This project uses API calls to generate weather data for multiple locations all over the world. The goal is to see how the weather changes as we approach the equator. Then, using the generated graphs I built a simple webpages displaying a weather analysis based on latitude. 

https://kasiakalemba.github.io/Weather-Analysis/
![](images/page.png)

## Technologies
* Language: Python - version 3.7
* Web design: HTML, CSS, Boostrap 
* Data Extraction & Exploration: Jupyter notebook, Pandas, Numpy
* Requests
* Citypy 
* Google maps & Places

## Weather Analysis
I visualized the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
[Jupyter Notebook](https://nbviewer.jupyter.org/github/kasiakalemba/API-Weather-Analysis/blob/master/WeatherPy/WeatherPy.ipynb)

![](images/city.png)

First I created a series of scatter plots to showcase the following relationships:
* Temperature (F) vs. Latitude
![](images/Fig1.png)

* Humidity (%) vs. Latitude
![](images/Fig2.png)

* Cloudiness (%) vs. Latitude
![](images/Fig3.png)

* Wind Speed (mph) vs. Latitude
![](images/Fig4.png)

Second I ran linear regression on each relationship: 
* Northern Hemisphere and Southern Hemisphere 
* Then creating a multiple linear regression plots. 

## Destination Selection
I created a heat map that displays the humidity for every city from part I. Using those cities, I narrowed them down to my favorite weather conditions and choose an ideal vacation spot. Then based on that location, using Google places API, I found the closest hotel to that city. 
[Jupyter Notebook](https://github.com/kasiakalemba/API-Weather-Analysis/blob/master/VacationPy/VacationPy.ipynb)

![](images/hotels.png)
![](images/map.png)

## Webpage: Latitude Analysis Dashboard
In building this dashboard, I created individual pages for each plot and a means to navigate between them. These pages contain the visualizations and their corresponding explanations. I built a landing page, where we can see a comparison of all of the plots, and another page where we can view the data used to build them.

![](images/graphs.png)


















