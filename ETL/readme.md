# Extract Transform Load folder
## Overview
This folder contains four jupyter notebooks containing the code used throughout the ETL process. The notebooks iterate on each other as the ETL process is worked through. The ETL_create_database notebook contains the final ETL code.

### ETL Function Test
The "ETL_function_test" notebook contains a function that reads in three data files; a Wikipedia JSON file, a movie metadata file from Kaggle, and MovieLens rating data from Kaggle. The purpose of this notebook was to test that the function was working properly.


### ETL Clean Wiki Movies
The "ETL_clean_wiki_movies" notebook code reads in the data sources and cleans the wikipedia json data. Redundant columns are combined, alternate titles are cleaned up, dollar amounts in various columns are standardized, date format is standardized, and the run time column is cleaned.

### ETL Clean Kaggle Movies
The "ETL_clean_kaggle_movies" notebook adds on to the code in the previous notebook to read in the kaggle data and clean it.

### ETL Create Database
The "ETL_create_database" notebook expands on the previous notebook and imports the cleaned files into a connected SQL database.