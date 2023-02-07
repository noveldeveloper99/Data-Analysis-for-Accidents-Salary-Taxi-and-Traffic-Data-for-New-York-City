# H9DAP-Database-and-Analytics-Programming
Project repository for Semester 1 Module using Python, PostgreSQL, MongoDB for XML, CSV, JSON files

# Data Analysis for Accidents, Salary, Taxi and Traffic Data for New York City #

This project renders a critical analysis of Traffic related data in New York City to understand the problems caused by the Traffic and to suggest possible measures to curb the same. 

### Datasets
For this project, four related datasets were analyzed to get an understanding on the Traffic scenario of New York City. Following are the links to the datasets used in the project
1. [New York Taxi](https://www.kaggle.com/datasets/oguzhantanrikulu/nytaxi?select=data-sample_data-nyctaxi-trips-2012-json_corrigido.json)  
2. [New York City Traffic](https://data.ny.gov/Transportation/Annual-Average-Daily-Traffic-AADT-Beginning-1977/6amx-2pbv)
3. [NYPD Accidents](https://www.kaggle.com/datasets/new-york-city/nypd-motor-vehicle-collisions?select=nypd-motor-vehicle-collisions.csv)
4. [Public Sector Salary](https://www.kaggle.com/datasets/new-york-state/nys-salary-information-for-the-public-sector?select=salary-information-for-industrial-development-agencies.csv)

### Technologies 
##### Programming Editor 
- Jupyter notebook
##### Database
- MongoDB database 
- PostgreSQL database
##### Programming Languages and libraries 
 
Python Language was primarily used in this project for analyzing the datasets. Along with Python, following Python Libraries and packages were also used:
   - Pymongo - for extracting data from MongoDB database
   - SQLAlchemy - for establishing connection with PostgreSQL database
   - Psycopg2 - for storing and extracting data from PostgreSQL database
   - Pandas - for  manipulating dataframes 
   - Plotly - for visualizing the analytics and results

   Steps to run the codes
   
   Prerequisites : IDE - Jupyter Notebook; Python Libraries - Pandas, Numpy, SQLAlchemy, Psycopg2, Datetime, Plotly, Matplotlib, Pymongo, XML; DB - MongoDB and          PostgreSQL.

a. For New_York_Taxi.ipynb file
  
  1. Download the dataset -New_York_Taxi_Trips.
  2. Create a Database and its Collection in MongoDB Database and import the data using the GUI of MongoDB. (PS: The dataset of New York Taxi has no comma separating   the instances, hence if you try to import this dataset using python, you will get an error regarding the file content Since there are 1 million instances in the     dataset, it was not feasible to manually add comma to separate the instance on the JSON file. Hence GUI approach of MongoDB was used to load the data into the       database).
  3. Create a Database in the PostgreSQL database.
  4. Run the file cell-by-cell (Since the dataset is huge, it is recommended to run cell-by-cell. Also it may take some time to execute).
  5. In ‘Storing the Processed and Structured Data in PostgreSQL’ of the code’ Configure the following line as per the configuration of the system. 
     
     'connection = create_engine('postgresql://postgres:admin@localhost:5432/dap')'
  
     In case of, postgres - write the username of your PostgreSQL database admin - write the password of your PostgreSQL database dap - write the name of the              database that was created in Step 3.
  6. Post the configuration of Step 5, keep running the code line by line.
  
b. For XMLTrafficdata.ipynb file

  1. Download the dataset - New York City Traffic.
  2. Create a Database in the PostgreSQL database.
  3. Run the file cell-by-cell (Since the dataset is huge, it is recommended to run cell-by-cell. Also it may take some time to execute).
  4. Configure the following line as per the configuration of the system.
    
     'connection = create_engine('postgresql://postgres:admin@localhost:5432/dap')'
     
  5. In case of, postgres - write the username of your PostgreSQL database admin - write the password of your PostgreSQL database dap - write the name of the              database that was created in Step 2.
  6. Post the configuration of Step 4, keep running the code line by line.

c. For Accidents_and_Salary_data_Final_EDA_v2.ipynb file

  1. Download the datasets - NYPD Accidents and Public Sector Salary.
  2. Create a Database in the PostgreSQL database.
  3. Run the file cell-by-cell (Since the dataset is huge, it is recommended to run cell-by-cell. Also it may take some time to execute)
  4. Configure the following line as per the configuration of the system.
     
     'connection = create_engine('postgresql://postgres:admin@localhost:5432/dap')'     
     
  5. In case of, postgres - postgres - write the username of your PostgreSQL database admin - write the password of your PostgreSQL database dap - write the name of      the database that was created in Step 2.
  6. Post the configuration of Step 4, keep running the code line by line.
