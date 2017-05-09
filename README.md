# Bike-Sharing-Rides

## Project description
Predict the number of riders according to historical data using simple neural networks, implemented using raw python and numpy.

## Dataset 
Bike sharing rental process is highly correlated to the environment and seasonal setting. For example, weather conditions, season, day of week, hour of the day, etc.
Therefore, the datasets 'hour.csv' and 'day.csv' are aggregated from two datasets on two hourly and daily basis. One of these two datasets is the two-year historical log corresponding to years 2011 and 2012 from Capital Bikeshare system, Washington D.C. USA, which is publicly available in http://capitalbikeshare.com/system-data. The other one is the dataset of weather information extracted from http://www.freemeteo.com.

## Files
1. hour.csv: bike sharing counts aggregated on hourly basis. Records: 17379 hours.
2. day.csv: bike sharing counts aggregated on daily basis. Records: 731 days.
3. 3-layer_nueral_network.ipynb: nueral network implementation on jupyter notebook.

## Dataset characteristics
instant: record index
dteday: date
season: 1:spring, 2:summer, 3:fall, 4:winter
yr: year(0: 2011, 1:2012)
mnth: month
holiday: the day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
weekday : day of the week
workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
temp : Normalized temperature in Celsius. The values are divided to 41 (max)
atemp: Normalized feeling temperature in Celsius. The values are divided to 50 (max)
hum: Normalized humidity. The values are divided to 100 (max)
windspeed: Normalized wind speed. The values are divided to 67 (max)
casual: count of casual users
registered: count of registered users
cnt: count of total rental bikes including both casual and registered
