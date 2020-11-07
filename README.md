# SQL Challange

<h1>EMPLOYEES SQL DATABASE</h1>

<h2>Introduction</h2>
The project requires that taking into account (6) CSV data files, to create and map a SQL Database solution. Once the database sturcture is completed the data must be uploaded and then queried to answer questions about the data contained within. Below is a diagram of the database. Please note: some minor changes were made post image capture.


!["DB Schema Diagram"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Schema/DB_Schema.png)


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


!["Question 1 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_1.png)

<li>List first name, last name, and hire date for employees who were hired in 1986.</li>


!["Question 2 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_2.png)

<li>List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.</li>


!["Question 3 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_3.png)

<li>List the department of each employee with the following information: employee number, last name, first name, and department name.</li>


!["Question 4 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_4.png)

<li>List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."</li>


!["Question 5 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_5.png)

<li>List all employees in the Sales department, including their employee number, last name, first name, and department name.</li>


!["Question 6 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_6.png)

<li>List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.</li>


!["Question 7 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_7.png)

<li>In descending order, list the frequency count of employee last names, i.e., how many employees share each last name.</li>


!["Question 8 Query Output Sample"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Question_8.png)

</ol>

<h2> Bonus </h2>

<ol>
<li>Average Salary by Employee Count (Histogram).</li>

!["Histogram Salary by Title"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/Salary_Histogram.png)

<li>Average Salary by Employee Title.</li>

!["Average Salary by Title"](https://github.com/timsamson/sql_challange/blob/main/EmployeeSQL/Images/AVG_Salary_by_Title.png)

</ol>









