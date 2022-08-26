The WeatherPy code takes 1500 random cities and checks for unique cities.
Once they have been verified, the raw data will be cleaned to reflect the city names, latitude, longitude, weather, and the country it resides in.

Latitude is plotted against temperature, humidity, cloudiness, and wind speed. Regression lines and r values are also generated.
This is done for Northern and Southern hemispheres (Latitude > 0 and < 0)

In the VacationPy code, the csv file from WeatherPy is loaded in and a heatmap is generated from the cities listed.
Based on these criteria:

A max temperature lower than 80 degrees but higher than 70.

   * Wind speed less than 10 mph.

   * Zero cloudiness.

   * Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

the dataframe is narrowed down to a smaller subset of cities.
API keys are used to find hotels nearby. Any city without a hotel nearby is removed from the dataframe.
Markers are then dropped onto the map with the hotel location and information provided.