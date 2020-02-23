# World_Weather_Analysis
#Outline of Project Plan

	•	Task: Collect and analyze weather data across cities worldwide.
	•	Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients’ weather preferences.
	•	Method: Create a Pandas DataFrame with 500 or more of the world’s unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data.
Analysis of the data is split into three main parts, or stages.

	1.	Collect the Data
	◦	Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
	◦	Use the citipy module to list the nearest city to the latitudes and longitudes.
	◦	Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
	◦	Parse the JSON data from the API request.
	◦	Collect the following data from the JSON file and add it to a DataFrame:
	▪	City, country, and date
	▪	Latitude and longitude
	▪	Maximum temperature
	▪	Humidity
	▪	Cloudiness
	▪	Wind speed
  
	2.	Exploratory Analysis with Visualization
	◦	Create scatter plots of the weather data for the following comparisons:
	▪	Latitude versus temperature
	▪	Latitude versus humidity
	▪	Latitude versus cloudiness
	▪	Latitude versus wind speed
	◦	Determine the correlations for the following weather data:
	▪	Latitude and temperature
	▪	Latitude and humidity
	▪	Latitude and cloudiness
	▪	Latitude and wind speed
	◦	Create a series of heatmaps using the Google Maps and Places API that showcases the following:
	▪	Latitude and temperature
	▪	Latitude and humidity
	▪	Latitude and cloudiness
	▪	Latitude and wind speed
  
	3.	Visualize Travel DataCreate a heatmap with pop-up markers that can display information on specific cities based on a customer’s travel preferences. Complete these steps:
	◦	Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
	◦	Create a heatmap for the new DataFrame.
	◦	Find a hotel from the cities’ coordinates using Google’s Maps and Places API, and Search Nearby feature.
	◦	Store the name of the first hotel in the DataFrame.
	◦	Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.
	
Code Files:
WeatherPy.ipynb
VacationPy.ipynb

Data Folder:
cities.csv
.png image files of images

New Dataframe Image:
![alt text](https://github.com/Al-Huneidi/World_Weather_Analysis/blob/master/screenshots/Part_1_Dataframe.png)


## WeatherPy Challenge Objectives


	•	Use nested try-except blocks.
	•	Use Pandas methods and attributes on a DataFrame or Series.
	•	Create a new DataFrame from a new API search with new weather parameters.
	•	Filter DataFrames based on input and nested decision statements, and logical expressions.
	•	Create pop-up markers on a Google map from a filtered DataFrame.
	•	Add a directions layer on a Google map between cities in the filtered DataFrame.

### Part 1 Instructions - Get the Weather Description and Amount of Precipitation for Each City

	1.	Create a new Jupyter Notebook file and name it Weather_Database.ipynb.
	2.	Generate a new set of 1,500 random latitudes and longitudes.
	3.	Get the nearest city using the citipy module.
	4.	Perform an API call with the OpenWeatherMap.
	5.	Retrieve the following information from the API call:
	◦	Latitude and longitude
	◦	Maximum temperature
	◦	Percent humidity
	◦	Percent cloudiness
	◦	Wind speed
	◦	Weather description (e.g., clouds, fog, light rain, clear sky)
	◦	Using a try-except block, if it is raining, get the amount of rainfall in inches for the last three hours. If it is not raining, add 0 inches for the city.
	◦	Using a try-except block, if it is snowing, get the amount of snow in inches for the last three hours. If it is not snowing, add 0 inches for the city.
	6.	Add the data to a new DataFrame.
	7.	Save the new DataFrame as a CSV file to be used for Part 2.
	8.	Upload the CSV file as part of your submission as WeatherPy_challenge.csv.
	9.	Answer this question using Pandas methods: How many cities have recorded rainfall or snow?
		64 cities have rainfall.
		27 cities have snowfall.

New DataFrame Image:
!{alt text] (https://github.com/Al-Huneidi/World_Weather_Analysis/blob/master/screenshots/Part_1_Dataframe.png)

### Part 2 Instructions - Have Customers Narrow Their Travel Searches Based on Temperature and Precipitation
	1.	Create a new Jupyter Notebook file and name it Vacation_Search.ipynb.
	2.	Import the WeatherPy_vacation.csv file from Part 1 as a new DataFrame.
	3.	Filter the DataFrame for minimum and maximum temperature preferences, and if the rain or snow accumulation is 0 inches or not using conditional statements. Do the following:
	◦	Prompt the customer for the minimum temperature preference.
	◦	Prompt the customer for the maximum temperature preference.
	◦	Prompt the customer to answer if he or she would like it to be raining or not, using input("Do you want it to be raining? (yes/no) ").
	◦	Prompt the customer to answer if he or she would like it to be snowing or not, using input("Do you want it to be snowing? (yes/no) ").
	4.	Add the cities to a marker layer map with a pop-up marker for each city that includes:
	◦	Hotel name
	◦	City
	◦	Country
	◦	Current weather description with the maximum temperature
	5.	Save and upload the new DataFrame as WeatherPy_vacation.csv.
	6.	Save and upload the new marker layer map as WeatherPy_vacation_map.png.

First 5 rows of Hotel DataFrame Image:
![alt text](https://github.com/Al-Huneidi/World_Weather_Analysis/blob/master/screenshots/Part_2_dataframe.png)

Marker Layer Map Image:
![alt text](https://github.com/Al-Huneidi/World_Weather_Analysis/blob/master/screenshots/WeatherPy_vacation_map.png)

Pop-up Marker Map for Each City Image:


### Part 3 Instructions - Create a Travel Itinerary with a Corresponding Map
Create a map (travel itinerary) that shows the route between four cities from the customer’s possible travel destinations, and then create a map with pop-up markers for the four cities.

Vacation Itinerary Map Image:


Code files:
Weather_Databas.ipynb
Vacation_Search.ipynb
Vacation_Itinerary.ipynb

Data Folder:
WeatherPy_challenge.csv
WeatherPy_vacation.csv

Image Folder:
WeatherPy_vacation_map.png
WeatherPy_travel.map.png
WeatherPy_travel_map_markers.png

