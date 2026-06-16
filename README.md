📊 Data Analysis Project Using Python & SQL
🚀 Project Overview

This project demonstrates a complete ETL (Extract, Transform, Load) workflow using Python, Pandas, SQLAlchemy, Microsoft SQL Server, and Kaggle API.

The objective was to download a dataset from Kaggle, clean and preprocess the data using Pandas, and load the transformed dataset into SQL Server for further analysis and reporting.

🛠️ Tools & Technologies
Python
Pandas
SQLAlchemy
Microsoft SQL Server
Kaggle API
Jupyter Notebook
📂 Project Workflow
Phase 1: Data Acquisition
Download dataset using Kaggle API
Extract ZIP files
Load dataset into Pandas DataFrame
Phase 2: Data Cleaning & Preprocessing
Handle missing values
Remove duplicate records
Convert data types
Create new columns
Filter and transform data
Phase 3: Data Loading
Connect to SQL Server using SQLAlchemy
Load cleaned data into SQL Server
Verify data loading using SQL queries
🔄 ETL Process
Extract
   ↓
Download Data from Kaggle API
   ↓
Load Data into Pandas
   ↓
Clean & Transform Data
   ↓
Connect SQL Server using SQLAlchemy
   ↓
Load Data into Database
   ↓
Validate Data
📊 Data Cleaning Tasks

✔ Handled missing values

✔ Removed duplicate records

✔ Converted columns to appropriate data types

✔ Created new calculated columns

✔ Filtered unnecessary records

✔ Validated final dataset

💾 Loading Data into SQL Server
from sqlalchemy import create_engine

engine = create_engine(
    "mssql+pyodbc://SERVER_NAME/DATABASE_NAME?driver=ODBC+Driver+17+for+SQL+Server"
)

df.to_sql(
    'table_name',
    con=engine,
    if_exists='append',
    index=False
)
🎯 Key Skills Demonstrated
Data Extraction using Kaggle API
Data Cleaning with Pandas
Data Transformation
Database Connectivity using SQLAlchemy
SQL Server Data Loading
ETL Pipeline Development
Data Validation
📚 Learning Outcomes

Through this project, I gained practical experience in:

Building an ETL pipeline
Working with real-world datasets
Cleaning and transforming data using Pandas
Connecting Python with SQL Server
Loading large datasets into databases
Verifying data quality after loading
👨‍💻 Author

Sourav Bhattacharya

Data Analyst | SQL | Python | Power BI | Excel

⭐ If you found this project helpful, please consider giving it a star on GitHub.

This version looks professional and is suitable for GitHub recruiters and hiring managers.
