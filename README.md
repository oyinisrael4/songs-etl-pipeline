# songs-etl-pipeline
ETL pipeline extracting 10,000 song records from MySQL, cleaning data and migrating to PostgreSQL
# Songs ETL Pipeline

## What This Project Is About
This was a hands-on project where I connected Python 
to a MySQL database, pulled out 10,000 song records, 
cleaned the messy data and moved it into PostgreSQL. 
I also saved the final data in different file formats.

## What I Actually Did
- Pulled 10,000 raw song records from a MySQL database
- Found and removed 5,309 songs with year recorded as 0
- Removed 12 songs where tempo was recorded as 0
- Removed 5 songs with incorrect loudness values
- Changed data types to reduce memory usage
- Loaded the cleaned 4,674 records into PostgreSQL
- Saved the data as CSV, Parquet, Pickle and Excel files

## What I Learned
Working on this project taught me how messy real data 
can be. Over half the records had invalid year values 
which I had to identify and remove before the data 
was usable. I also learnt the difference between 
connecting to a database directly vs using SQLAlchemy 
and why SQLAlchemy is the better approach.

## Technologies Used
Python, pandas, SQLAlchemy, MySQL, 
PostgreSQL, pyarrow, Jupyter Notebook
