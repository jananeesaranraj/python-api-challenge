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

* The scatter plot between city latitude and max temperature shows that as the latitude increases from the equator, the max temperature decreases.Latitude is inversely proportional to temperature.

**Humidity (%) vs. Latitude**

![City_Lat_Humidity](https://user-images.githubusercontent.com/112193116/197406196-5aa24f34-c0cc-49f8-ba2c-38c67a8189a0.png)

* The scatter plot shows that there seems to be no direct relationship between latitude and humidity. Humidity% of most of the cities are found to be above 60%.There are only very limited number of cities located in area with humidity below 20%.

**Cloudiness (%) vs. Latitude**

![City_Lat_Cloudiness](https://user-images.githubusercontent.com/112193116/197406194-aac8beb7-0837-4ef7-8506-18d003a92fc9.png)

* The scatter plot shows that there is no Correlation seen between the latitude and cloudiness from the above plot.The data points are more concentrated at 100%, 0%, also evenly across all latitudes.

**Wind Speed (mph) vs. Latitude**

![City_Lat_WindSpeed](https://user-images.githubusercontent.com/112193116/197406199-75bd2e58-1d1e-467f-8881-8320c6701de5.png)

* The scatter plot shows that most cities have wind speed less than 15mph.There is no strong relationship between the wind speed and latitude from the above plot

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

**Northern Hemisphere: Temperature (F) vs. Latitude**

**Southern Hemisphere: Temperature (F) vs. Latitude**

![Latitude_Temp_North](https://user-images.githubusercontent.com/112193116/197406355-ac725a32-39a5-4362-adce-e1d06630a35d.png)

![Latitude_Temp_South](https://user-images.githubusercontent.com/112193116/197406356-af809a24-527a-4747-8bfc-8274b78ca98d.png)

* In the Northern Hemisphere,the rvalue is 0.7513578529149185. It shows that there is strong Corelation between the Latitude and the Max Temperature.The linear regression line shows that lower the latitude,higher the temperature.
* In the Southern Hemisphere,the rvalue is 0.4310417236065775.It shows the Correlation between the latitude and Max temperature is Moderate and it is positive Corelation,which means the higher the latitude (closer the equator line) the higher the temperature.

**Northern Hemisphere: Humidity (%) vs. Latitude**

**Southern Hemisphere: Humidity (%) vs. Latitude**

![Latitude_Humidity_North](https://user-images.githubusercontent.com/112193116/197406353-283fb26e-7b0c-4923-ac51-856adf474dbe.png)

![Latitude_Humidity_south](https://user-images.githubusercontent.com/112193116/197406354-e8eed730-7ef0-4728-b92c-76f91f2bf0f4.png)

* As per the above figure,the correlation between latitude and percentage of humidity in both northeren hemisphere and southern hemisphere seems to be very weak as the rvalues are very low.

**Northern Hemisphere: Cloudiness (%) vs. Latitude**

**Southern Hemisphere: Cloudiness (%) vs. Latitude**

![Latitude_Cloud_North](https://user-images.githubusercontent.com/112193116/197406351-64cfaa66-868e-464f-a2c2-811a51596a72.png)

![Latitude_Cloud_South](https://user-images.githubusercontent.com/112193116/197406352-d94db7f4-8c5c-4eb8-bb85-4e6f1afe63ab.png)

* The rvalues for northern and southern hemisphere seems to be low,which means the correlation between the latitude and the cloudiness is very weak. Linear regression lines and the low r-squared values in both graphs indicate that latitude might not be a significant factor that causes cloudiness.

**Northern Hemisphere: Wind Speed (mph) vs. Latitude**

**Southern Hemisphere: Wind Speed (mph) vs. Latitude**

![Latitude_Wind_North](https://user-images.githubusercontent.com/112193116/197406357-c5bb7351-0d67-4ce0-a991-00f391278e8f.png)

![Latitude_Wind_South](https://user-images.githubusercontent.com/112193116/197406359-36161a76-6c22-4788-95f2-4b6d11d6a896.png)

*The rvalues for northern and southern hemisphere seems to be very low,which means the correlation between the latitude and the wind speed is very weak.The regression lines and rvalues indicate that wind speed could not be predicted by the latitude.

**Part 2: VacationPy**

Now, use your weather data skills to plan future vacations. Use Jupyter gmaps and the Google Places API for this part of the assignment.

1.Create a heat map that displays the humidity for every city

![Humidity_Heatmap](https://user-images.githubusercontent.com/112193116/197406348-859d3f16-5fc4-4d20-b593-f28d9488d381.png)

2.Plot the hotels on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country,

Here is the map shown the cities with maximum temperature between 70 and 80 degrees fahrenheit, wind speed less than 10 mph, zero percent cloudiness.

![Hotel_list_Heatmap](https://user-images.githubusercontent.com/112193116/197406343-7c745faf-1f48-4a98-9144-660eb7814d37.png)
