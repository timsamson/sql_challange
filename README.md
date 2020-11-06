# SQL Challange

<h1>EMPLOYEES SQL DATABASE</h1>

<h2>Introduction</h2>

<h4>WeatherPY</h4>
The Python API challange looks at random latitudes and longutudes to determine city locations. That data is then used to find the curretn weather (at the time of the API calls) from OpenWeather. The resulting data is then analyised with linear regression to determine if there is coorelation between four data points and thier location on with the Northern of Southern Hemisphere.
<h4>VacationPY</h4>
VacationPy then looks at teh Humidity data from the WeatherPY exercise and plots the data as a heatmap using Google Maps API. The data is additionally sorted via my ideal vacation location conditions as determined my me. Once the lolcation list is created, Google places API is called to determine the closest hotel to that location, if a location did not have a hotel within 5000 meters it was then dropped form the dataframe. The locations and names of the hotels were then overlayed onto the google heatmap as a layer. 

<h2>Technologies</h2>

<ul><li>Python 3.6</li>
<li>Jupyter Notebook</li>
<li>Postgres</li>
<li>QuickDatabaseDiagrams.com</li>
<li>Pandas</li></ul>

<h2>Dependencies</h2>
<ul><li>MatPlotLib</li>
<li>Sqlalchem</li>
<li>Psycopg2</li>
<li>Numby</li></ul>

<h2>General Notes</h2>

Repo contains folder "EmployeeSQL"

Interior folders are:
<ul><li>Data</li>
<li>Queries</li>
<li>Images</li>
<li>Schema</li></ul>

Additional"Files" folder whith Jupyter notebooks and associated resources:
Please use notebooks titled:
 
<ul><li><b>WeatherPy.ipynb</b></li>
  <li><b>vacationPy.ipynb</b></li></ul>
  
<h2>API Keys and Installation</h2>

Please note that to run the code, the user will need to imput thier own api keys for both openweather and goodle maps in the file: api_keys.py. Failure to do so will rsult in errors in both notebooks. 

<h2>Observation and Analysis</h2>

<h2> Scatter Plots </h2>

!["Latitude Vs. Wind"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Latitude%20vs.%20Wind%20Speed.png)

!["Latitude Vs. Cloudiness (%)"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Latitude%20vs.%20Cloudiness.png)

!["Latitude Vs. Humidity (%)"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Latitude%20vs.%20Humidity.png)

!["Latitude Vs. Max Temp"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Latitude%20vs.%20MAX%20Temperature.png)

<h2> Linear Regression Plots </h2>
<h3> Max Temp</h3>

!["Northern Hemisphere | Max Temp vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Northern%20Hemisphere%20%7C%20Max%20Temp%20vs.%20Latitude%20Regression.png)

Northern Hemisphere | Max Temp vs. Latitude

The r-squared is : -0.88

Temperature decreases as you move south from the equator. There is a strong linear coorelation.

!["Southern Hemisphere | Max Temp vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Southern%20Hemisphere%20%7C%20Max%20Temp%20vs.%20Latitude%20Regression.png)

Southern Hemisphere | Max Temp vs. Latitude

The r-squared is : 0.75

Temperature decreases as you move north from the equator. There is a strong linear coorelation. 

<h3>Humidity</h3>

!["Northern Hemisphere | Humidity (%) vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Northern%20Hemisphere%20%7C%20Humidity%20(%25)%20vs.%20Latitude%20Regression.png)

Northern Hemisphere | Humidity vs. Latitude

The r-squared is : 0.27

The coorelation between humidity and latitude is weak in the Northen hemisphere.  

!["Southern Hemisphere | Humidity (%) vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Southern%20Hemisphere%20%7C%20Humidity%20(%25)%20vs.%20Latitude%20Regression.png)

Southern Hemisphere | Humidity vs. Latitude

The r-squared is : 0.15

The coorelation between humidity and latitude is weak in the Southern hemisphere. 

<h3>Cloudiness</h3>

!["Northern Hemisphere | Cloudiness (%) vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Northern%20Hemisphere%20%7C%20Cloudiness%20(%25)%20vs.%20Latitude%20Regression.png)

Northern Hemisphere | Cloudiness vs. Latitude

The r-squared is : 0.2

The coorelation between cloudiness and latitude does not exsist. 

!["Southern Hemisphere | Cloudiness (%) vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Southern%20Hemisphere%20%7C%20Cloudiness%20(%25)%20vs.%20Latitude%20Regression.png)

Southern Hemisphere | Cloudiness vs. Latitude

The r-squared is : 0.15

The coorelation between cloudiness and latitude is a weak coorelation. 

<h3> Wind Speed</h3>

!["Northern Hemisphere - Wind Speed (mph) vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Northern%20Hemisphere%20-%20Wind%20Speed%20(mph)%20vs.%20Latitude%20Regression.png)

Northern Hemisphere | Wind Speed vs. Latitude

The r-squared is : 0.05

The coorelation between Wind Speed and latitude does not exsist.

!["Southern Hemisphere - Wind Speed (mph) vs. Latitude"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/Southern%20Hemisphere%20-%20Wind%20Speed%20(mph)%20vs.%20Latitude%20Regression.png)

Southern Hemisphere | Wind Speed vs. Latitude

The r-squared is : -0.08

The coorelation between Wind Speed and latitude does not exsist. 

<h2> VacationPY </H2>

Google heatmap showing humidity data as a heatmap from previous exercise WeatherPy

!["Humidity Heatmap"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/vacation_humidity_heatmap.png)

Hotel overlay showing my most ideal vacation locations.

<ul><li>Wind Speedless than or equal to 10 MPH</li>
 <li>Cloudiness less than 10%</li>
<li>Humidity less than 35%</li>
<li>Temperature between 60 and 95 degress F. </li></ul>

!["Hotel Overlay"](https://github.com/timsamson/Python_API_Challange/blob/main/Files/images/vacation_hotel_overlay.png)













