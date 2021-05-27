# rice-btcmp-hw6-python-api-challenge
## Project objective

Use Python requests, APIs and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

## Part I - WeatherPy

Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator, utilizing [CitiPy Python library](https://pypi.python.org/pypi/citipy) & [OpenWeatherMap API](https://openweathermap.org/api) to create a representative model of weather across world cities.

Code produces a series of scatter plots to showcase the following relationships:

- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

Run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- Northern Hemisphere - Humidity (%) vs. Latitude
- Southern Hemisphere - Humidity (%) vs. Latitude
- Northern Hemisphere - Cloudiness (%) vs. Latitude
- Southern Hemisphere - Cloudiness (%) vs. Latitude
- Northern Hemisphere - Wind Speed (mph) vs. Latitude
- Southern Hemisphere - Wind Speed (mph) vs. Latitude

Include a print log of each city as it's being processed with the city number & city name and save a CSV file of all retrieved data and a PNG images for the scatter plots.

### Part II - VacationPy

Use retrieved weather data to plan future vacations using <i>jupyter-gmaps</i>i and the <i>Google Places API</i>.

- Create a heat map that displays the humidity for every city from the *Part I* of the homework.
- Narrow down the DataFrame to find your ideal weather condition. For example:
  - Using a [min, max] range for temperature.
  - Maximum wind speed.
  - Maximum cloudiness.
  - Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.
- Use Google Places API to find the first hotel for each city located within 5000 meters of given set of coordinates.
- Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

### Input data:

No input data is provided, as city locations are to be generated randomly.

### Observations:

