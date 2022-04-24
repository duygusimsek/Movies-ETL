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

* Wikipedia and Kaggle website data were extracted in JSON and CSV formats with an ETL function.
* The data from the Wikipedia JSON and Kaggle metadata were converted into Pandas data frames and displayed in the [ETL_function_test.ipynb](https://github.com/duygusimsek/Movies-ETL/blob/main/ETL_function_test.ipynb) file.
* The MovieLens rating data was converted to Pandas data frame and displayed. 

* The  TV shows were filtered out from the movie list and a data frame was created. 
* To catch errors while extracting the IMDb IDs with a regex and dropping duplicate IDs a try-except block was used. 
* The extraction and transformation of the Wikipedia data in the ETL function were completed. 
* Some columns’ names were reorganized and changed. 
* Some columns were cleaned in the Wikipedia data frame. 
* The cleaned Wikipedia data was converted to a Pandas DataFrame and displayed in the [ETL_clean_wiki_movies.ipynb](https://github.com/duygusimsek/Movies-ETL/blob/main/ETL_clean_wiki_movies.ipynb) file.

* By using the ETL function the extraction and transformation of the Kaggle metadata were completed. 
* The Kaggle metadata was cleaned and merged with the Wikipedia dataset. 
* Unnecessary columns were dropped and the missing Kaggle data were filled. 
* The ‘movies_with_ratings_df’ and ‘movies_df’ data frames displayed in the [ETL_clean_kaggle_data.ipynb](https://github.com/duygusimsek/Movies-ETL/blob/main/ETL_clean_kaggle_data.ipynb) file.

* ‘movies_df’ data frame replaces the current data in the movies table in the SQL database and the screenshot of the count of rows was saved as [movies_query.png](https://github.com/duygusimsek/Movies-ETL/blob/main/Resources/movies_query.png). 
* The MovieLens rating CSV file was added to the ratings table in the SQL database,  and the screenshot of the count of rows was saved as [ratings_query.png](https://github.com/duygusimsek/Movies-ETL/blob/main/Resources/ratings_query.png)
* The elapsed time to add the data to the database is displayed in the [ETL_create_database.ipynb](https://github.com/duygusimsek/Movies-ETL/blob/main/ETL_create_database.ipynb) file.


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


