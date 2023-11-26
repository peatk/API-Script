# Python API Challenge

## Background
Utilizing the OpenWeatherMap API & the GeoApify API create API requests, and develop weather models that prove the weather gets hotter the closer you are to the equator. This requires python requests, APIs, and json traversals to obtain the desired outcome. The excercise is broken into 2 parts - (1) WeatherPy, and 
(2) VacationPy. 

#####  WeatherPy
In this deliverable I created a Python script to visualize the weather of an array of randomized cities of varying distances from the equator. I used the citipy library to connect to the OpenWeatherMap API to create a representative model of weather across cities.

After developing the necessary code I created plots to showcase the relationship between the weather variables to the city's latitiude.
    - Latitude vs. Temperature
    - Latitude vs. Humidity
    - Latitude vs. Cloudiness
    - Latitude vs. Wind Speed
Then I computed the linear regression for each relationship. After separating the data into 2 sections northern (greater than or equal to 0 degrees latitude) and southern hemishphere (less than 0 degrees latitude), I plotted the linear regression line, the model's formula, and the r values. This allowed me to develop an analysis for each relationship which can be found in the WeatherPy code. 

##### VacationPy
In this deliverable I used my WeatherPy data to identify future travel. To do so the dataframe was output to a CSV file and imported with the weather and coordinates data for each city. Then I created a map to display a point for every city where the size of the point was the humidity. Then I narrowed down the results to my ideal weather - Temperature between 15-80 degress, and Humidity between 20-60. After narrowing these results I used the GeoApify API to find the hotel within a 10km radious and with closest proximity to the city's latitude and longitude. 

