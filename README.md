# WeatherPy
## Overview of the PlanMyTrip app

Overview of the PlanMyTrip app
This report presents the results of creating 2000 random locations (latitude and longitude) and setting an API request to get their weather. By using Python within the Jupyter Notebook and several dependencies (pandas, requests, gmaps, matplotlib, numpy and citipy), it was possible to create a database containing the name of the cities near each location. We got the data into DataFrames to create plots and we filtered the data according to the client's weather preferences to identify potential travel destinations and nearby hotels. Finally, we created a travel itinerary with four cities to visit.

### Folders/Files

1. Weather_Database
   Code: Weather_Database.ipynb
   CSV output: WeatherPy_Database.csv

2. Vacation_Search
   Code: Vacation_Search.ipynb
   CSV output: WeatherPy_vacation.csv
   Image: WeatherPy_vacation_map.png

3. Vacation_Itinerary
   Code: Vacation_Itinerary.ipynb
   Image1: WeatherPy_travel_map.png
   Image1: WeatherPy_travel_map_markers.png
   Image1: WeatherPy_travel_map_markers2.png

## Results

Three folders were created to hold the different jupyter notebooks to create and clean the database, filter the data and create plots, and create the itinerary. 

### The Weather Database

The weather database jupyter notebook uses the bumpy library to create a series of random numbers between -90 and 90 for latitudes and between -180 to 180 for longitudes. We used requests to get a list of cities near each coordinate created before. We gathered the weather information for those cities and we placed that into data frames. Finally, we exported it into a CSV file "WeatherPy_Database.csv"

### The Vacation Search

The vacation search jupyter notebook uses pandas, requests, and gmaps dependencies. We imported the csv file that was created in the previous notebook and we asked for some weather preferences (minimum temperature for the cities that are going to be along the route). We selected 4 cities to make the vacation plan. 

We filtered the data according to those preferences and we used a nearby search to gather the nearest hotel for each city. We added the hotel name in each city and we exported a second csv file "WeatherPy_vacation.csv".Finally, we plotted the locations with info box markers. 

![WeatherPy_vacation_map.png](https://github.com/DylanMontemayor/WeatherPy/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### The Vacations Itinerary

The Vacation Itinerary jupyter notebook uses pandas, requests, and gmaps. We imported the csv "WeatherPy_vacation.csv". We plotted the route for the vacations and we included the four locations' weather information markers. 

![WeatherPy_travel_map.png](https://github.com/DylanMontemayor/WeatherPy/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

![WeatherPy_travel_map_markers2](https://github.com/DylanMontemayor/WeatherPy/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers2.png)

## Summary

With this app, it is possible to add temperature parameters to filter possible cities to go to. The app will suggest a vacation itinerary with a route that includes four cities and it will show its location and weather information. 
