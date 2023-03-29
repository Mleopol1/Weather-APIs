# Weather APIs

This project is composed of two deliverables, WeatherPy and VacationPy. In WeatherPy, a Python script is used to visualize the weather of over 500 cities of varying distances from the equator. The [citipy Python library](https://pypi.python.org/pypi/citipy "citipy") and the [OpenWeatherMap API](https://openweathermap.org/api "OpenWeatherMap") are used to create a representative model of weather across cities. In VacationPy, the weather and coordinates data developed in WeatherPy are used to plan future vacations, using the geoViews Python library and the Geoapify API.

## WeatherPy

The WeatherPy deliverable fulfills the following requirements:

### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

Using the OpenWeatherMap API, the script retrieves weather data from the generated list of over 500 cities. A series of scatter plots are then created to showcase the following relationships:

   * Latitude vs. Temperature
   * Latitude vs. Humidity
   * Latitude vs. Cloudiness
   * Latitude vs. Wind Speed

### Requirement 2: Compute Linear Regression for Each Relationship

The plots are separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude), and the linear regression for each relationship is computed. A series of scatter plots are then created, including the linear regression line, the model's formula, and the r-values. The linear regression is explained and any relationships that are noticed or other findings are described.

## VacationPy

The VacationPy deliverable fulfills the following requirements:

1. **Create a map that displays a point for every city generated in WeatherPy:** The size of each point reflects the humidity of that city.

2. **Narrow down the cities to find your ideal weather condition:** The ideal weather condition was chosen to have a maximum temperature of between 70 and 80 degrees, a wind speed of less than 10 m/s, and zero cloudiness. These cities are then stored into a new DataFrame.

3. **For each city, find the nearest hotel:** For each city, the Geoapify API is used to find the first hotel located within 10,000 meters of the ideal cities' coordinates.

4. **Add the hotel name and the country as additional information in the hover message for each city on the map:** The final heatmap includes every city, with additional hover information for the five cities that met the ideal weather conditions.

![heatmap_with_markers](https://user-images.githubusercontent.com/111384049/228629958-43e74d17-aa44-42e9-81bc-4b80644e0585.PNG)

## Conclusion

The WeatherPy and VacationPy deliverables demonstrate the use of Python coding skills and calling of APIs to create a representative model of weather across cities and plan future vacations.
