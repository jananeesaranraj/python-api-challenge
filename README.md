# python-api-challenge
Python API Challenge
**Background**
Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"
Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?
**Part 1: WeatherPy**
In this section, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use a simple Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

**Temperature (F) vs. Latitude**

![City_Lat_Max_Temp](https://user-images.githubusercontent.com/112193116/197406197-b9fb8f67-1ac6-4d7f-9723-f363d0558009.png)

**Humidity (%) vs. Latitude**

**Cloudiness (%) vs. Latitude**

**Wind Speed (mph) vs. Latitude**

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

**Northern Hemisphere: Temperature (F) vs. Latitude**

**Southern Hemisphere: Temperature (F) vs. Latitude**

**Northern Hemisphere: Humidity (%) vs. Latitude**

**Southern Hemisphere: Humidity (%) vs. Latitude**

**Northern Hemisphere: Cloudiness (%) vs. Latitude**

**Southern Hemisphere: Cloudiness (%) vs. Latitude**

**Northern Hemisphere: Wind Speed (mph) vs. Latitude**

**Southern Hemisphere: Wind Speed (mph) vs. Latitude**


**Part 2: VacationPy**
Now, use your weather data skills to plan future vacations. Use Jupyter gmaps and the Google Places API for this part of the assignment.

1.Create a heat map that displays the humidity for every city

2.Plot the hotels on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country,
