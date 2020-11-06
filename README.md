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
<ul><li>Data- Copies of CSV Data files</li>
<li>Queries- Query File</li>
<li>Images- Charting Files</li>
<li>Schema- Shema File and PNG of Schema</li>
<li>Bonus- Jupyter Notebook for bonus work</li></ul>
  
<h2>API Keys and Installation</h2>

Please note that if you wish to recreate the SQL database using the schema contained within, the import order for the csv files should be done in the following order to avoid failures during upload:

<ul>
<li>departments</li>
<li>title</li>
<li>employees</li>
<li>salaries</li>
<li>dept_manager</li>
<li>dept_emp</li>
</ul>

<h2>Observation and Analysis- Sample Data Queries</h2>

<h2> Query Questions </h2>

<ol>
<li>List the following details of each employee: employee number, last name, first name, sex, and salary.</li>

<li>List first name, last name, and hire date for employees who were hired in 1986.</li>

<li>List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.</li>

<li>List the department of each employee with the following information: employee number, last name, first name, and department name.</li>

<li>List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."</li>

<li>List all employees in the Sales department, including their employee number, last name, first name, and department name.</li>

<li>List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.</li>

<li>In descending order, list the frequency count of employee last names, i.e., how many employees share each last name.</li>


</ol>

<h2> Bonus </h2>

<ol>
<li>Average Salary by Employee Count (Histogram).</li>

!["Histogram Salary by Title"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Salary_Histogram.png)

<li>Average Salary by Employee Title.</li>

!["Average Salary by Title"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/AVG_Salary_by_Title.png)

</ol>









