# Movies-ETL

## Overview

Raw data or primary data is collected in multiple places and forms. To perform any kind of data analysis, this data needs to be cleaned and structured. The data can be collated from one or more sources and it can also be outputted to one or more destinations. For this purpose, Extract, Transform, and Load (ETL) is the main concept in data engineering. It comes with many challenges. But with a proper ETL process, raw data can be consistent. Without a consistent data structure, it’s nearly impossible to perform any meaningful analysis.
 
### Purpose of the Analysis

A video streaming company wants to sponsor a hackathon where participants tried to predict which low-budget movies being released will become popular.  The data will be used as a data source and needs to be clean and organized to perform analysis.  In that order, the ETL process was used:

* Extracting data from two different sources
    * Wikipedia website web scrape for all movies released since 1990
    * Kaggle website data for rating data.
* Transforming data 
* Loading data using PostgreSQL,  saving the cleaned final data to pgAdmin. 


## Result 













## Resources

Data Sources:
 * Wikipedia web scrape JSON file
 * Kaggle data from Kaggle.com 
 * movies_metadata.csv
 * [ratings.csv](url)

Software:
 * Jupyter Notebook
 * PostgreSQL and PgAdmin

Language: [Python 3.10.2](https://www.python.org/downloads)


