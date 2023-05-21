# Python API Challenge

This repository contains the code and analysis for the Python API Challenge. The challenge consists of two parts: WeatherPy and VacationPy.

## WeatherPy

In the WeatherPy part, we analyze the weather of over 500 cities of varying distances from the equator. We use the citipy Python library to generate random geographic coordinates and find the nearest city to each latitude and longitude combination. Then, we retrieve weather data for these cities using the OpenWeatherMap API.

### Requirements

- Python 3.x
- Jupyter Notebook
- pandas
- requests
- citipy
- matplotlib
- scipy

### Weather Analysis

The WeatherPy.ipynb notebook performs the following analyses and creates corresponding plots:

1. Latitude vs. Temperature: This scatter plot shows the relationship between latitude and temperature. It helps visualize how temperature changes as we move away from the equator.
2. Latitude vs. Humidity: This scatter plot shows the relationship between latitude and humidity. It helps understand if there is any correlation between latitude and humidity levels.
3. Latitude vs. Cloudiness: This scatter plot shows the relationship between latitude and cloudiness. It helps analyze if there is any pattern in cloud cover across different latitudes.
4. Latitude vs. Wind Speed: This scatter plot shows the relationship between latitude and wind speed. It helps examine if there is any connection between latitude and wind speed.

For each relationship, linear regression analysis is performed for both the Northern Hemisphere and the Southern Hemisphere. The scatter plots with regression lines, equations, and correlation coefficients are also included in the notebook.

## VacationPy

In the VacationPy part, we use the weather data from WeatherPy to plan future vacations. We create maps using the geoViews Python library and the Geoapify API.

### Requirements

- Python 3.x
- Jupyter Notebook
- pandas
- matplotlib
- geopandas
- geoViews
- Geoapify


### Vacation 

The VacationPy.ipynb notebook performs the following tasks:

1. Creates a map with a point for every city in the city_data_df DataFrame. The size of the point represents the humidity level in each city.
2. Narrows down the city_data_df DataFrame based on the desired weather conditions.
3. Uses the Geoapify API to find the first hotel located within 10,000 meters of the coordinates for each city.
4. Adds the hotel name and country as additional information in the hover message for each city on the map.

## Acknowledgments

- [OpenWeatherMap](https://openweathermap.org/) for providing the weather data API.
- [Geoapify](https://www.geoapify.com/) for
