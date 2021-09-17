# Py Travel App

In this week project we are helping PlanMyTrip app to design a travel itinerary that includes four cities in the same country that can be travel by route. The four cities are chosen from a list of potential destinations that has been created based on the weather preferences of tester users. For this project, we are working with **Python** and **Pandas** in `jupyter notebook` and using *API* (Application Programming Interface) calls to two different websites: **OpenWeatherMap** and **Google Maps Platform**.

## Project Process:

In order to create the travel itinerary, we divide the process in three steps where relevant data is firstly gathered around the world.  Secondly and based on users' preferences, the information is filtered out such that only cities that meet certain temperatures conditions are considered. Lastly, and based on the second step, a route between four different cities is created.

![df](https://raw.githubusercontent.com/LeidyDoradoM/WorldWeather_Challenge/main/Weather_Database/df_citydata.png)
Table 1. World Weather DataFrame 


### 1. World-wide Weather

The first part of the project is related with the collection of weather conditions around the world. This is performed by generating a set of 2,000 random latitudes and longitudes, retrieve their nearest cities, perform an *API*  call to the **OpenWeatherMap** website. Extract information about temperatures, weather description for each one of the cities and then create a dataframe with all the updated weather data.

### 2. Potential Cities to Visit
 
 From the dataframe generated in the previous step and using an input statement to retrieve the customer weather preferences, we identify potential travel destinations and their nearby hotels. This relevant information is presented as a world map with markers and pop-up boxes showing city, hotel name, country, and current weather.

### 3. Final Travel Route

From the list of potential cities drawn in the second step, four cities are chosen and create a route between four cities using the **Google Directions API**. The final result is a route map with a marker layer and pop-up marker for each city on the itinerary.