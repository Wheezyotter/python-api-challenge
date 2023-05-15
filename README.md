# python-api-challenge
python-api-challenege is an exercise to practice retrieving JSON requests from APIs. 

To practice these skills, this script aims to collect weather data from OpenWeatherMap API to see how temperature, humidity, cloudiness, and wind speed change as you move towards the equator. The script then uses GEOapify to locate hotels in multiple cities that match a set of 'ideal' weather conditions as possible places to visit. 

### WeatherPy
---
In WeatherPy.ipynb a list of cities were created using citipy. Weather data from each listed city is retreived from OpenWeatherMap API. A series of scatter plots were then constructed to determine correaltion between latitude and series of weather variables. 

- Retrevied city weather data exported to as a CSV to the Data folder to be used elswehere. 

- All figures exported to the Figures folder in WeatherPy

### VacationPy
---
In VacationPy.ipynb, city weather data was imported from the WeatherPy CSV in the data folder and used to construct a global map of cities using hvplot. City point size determined by the humidity in each city. A set of criteria were created to find the 'ideal' weather conditions to visit:

- A temperature of 18C to 26C
- A humidity of 60 or below
- A cloud covered of 50% or below
- A wind speed of 1 - 5

A geopaify was used to find hotels in cities that fit the 'ideal' weather conditions and plotted on a map using hvplot. 

- City weather data sourced from cities.csv in the Data folder


----
Script was made for UCB Data Analytics Challenge 6

Author - Jacob Pohs

Some code used from provided Starter Code and stated within scripts.