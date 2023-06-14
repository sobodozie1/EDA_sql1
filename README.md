# <p><b>Exploratory Data Analysis With SQLite</b></p>

<img src="excel_img.png" alt="Excel logo" style="margin-left: auto; margin-right: auto; height: 100px; width: 100px;"/>

Exploratory data analysis (EDA) is an approach to analyzing data sets to summarize their main characteristics, often with visual methods. SQL is a powerful tool for data analysis and can be used for EDA.
The process of exploring a database starts by identifying the tables and the foreign keys that link them. Identifying missing values, counting the number of observations, and joining tables to understand relationships.Exploratory data analysis (EDA) with SQLite is a crucial step in understanding and gaining insights from data using SQLite database tool ⚙.
The dataset, Olympic Games Data, used here was got from Kaggle, and included a 120-year history of the beautiful sports ecumenism.

<p><b>Here are description of how to perform EDA with SQLite:</b></p>

  - Start by connecting to your SQLite database using a command-line interface or a GUI tool like SQLite Browser or DBeaver.
  - Retrieve an overview of the available tables in the database by executing the command <b>SELECT name FROM sqlite_master WHERE type='table';</b>.
  - Choose a specific table to analyze and run a query to fetch a sample of the data. For example, <b>SELECT * FROM tablename LIMIT 100;</b> retrieves the first 100 rows from the table.
  - Use the <b>PRAGMA table_info(tablename);</b> command to obtain information about the columns in the selected table, including their names, data types, and constraints.
  - Investigate, if needed, the distribution of numerical variables by executing queries such as <b>SELECT MIN(columnname), MAX(columnname), AVG(columnname) FROM tablename;</b>.
  - Calculate summary statistics for numeric columns using aggregate functions like <b>SUM, COUNT, AVG, MIN, and MAX</b> combined with the <b>GROUP BY</b> clause to analyze different subsets of data.
  - Explore the distribution of categorical variables by querying <b>SELECT columnname, COUNT(*) FROM tablename GROUP BY columnname;</b> to retrieve the frequency count for each unique category.
<p>Remember, SQLite is primarily a database engine, and while it provides powerful querying capabilities, some advanced EDA tasks may require exporting data to a dedicated statistical analysis tool or programming language like Python. And in this case Python via Jupyter Notebook was employed.</p>
