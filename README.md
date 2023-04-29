# python-api-challenge
Module 6 Challenge

Overall this challenge focuses on using APIs to collect random city locations from around the world, recording and graphing their current weather conditions, and then parsing that data based on the weather data to generate a list hotel locations in cities that meet the definded weather conditions.

The first task is to generate a list of random latitude and longitude locations across the entire globe and find corresponding cities close to these randomly generated locations. Each unique city that is located is added to a blank list defined as 'cities'.

The next task uses the generated list of cities and the Open Weather API (https://openweathermap.org/api) to collect the weather data for these cities from around the world. Using the API and I was able to pull specific information from the JSON data for each city such as latitude, longitude, maximum temperature, humdity, cloudiness, wind speed, country, and date. As the JSON data is looped through for each unique city within the 'cities' a collection of lists called 'city_data' a is populated. Then this collection of lists is converted into a Pandas dataframe named 'city_data_df'.

With the newly created dataframe I was able to generate scatter plots to show correlations between the latitude and the various weather information for each city.
The plot below is an example of the Max Temperature versus Latitude.

![City Latitude vs. Max Temperture](WeatherPy\output_data\City_Lat_vs_Max_Temp.png)