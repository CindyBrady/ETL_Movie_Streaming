# ETL_Movie_Streaming

![streaming.png](Images/streaming.png)

# Extract: your original data sources and how the data was formatted (CSV, JSON, pgAdmin 4, etc).
Pulled CSV files from kaggle (listed above)

# Transform: what data cleaning or transformation was required.
Dropped unnecessary columns listing things like (age, ID, year etc.)
Removed all null values
Reformatted columns for data consistency, numerical data was reformatted to decimals
Aggregated the data and found mean, and count of different streaming platforms (boolean to int)  
Output Director dataframe to CSV
Merged the two datasets on movie title and identified netflix originals  
Uploaded new merged netflix originals dataframe to postgres using SQL queries and connection engine
Selected data from the postgres database to confirm data and verify that data exists in the table

# Load: the final database, tables/collections, and why this was chosen.
We chose to load data to Postgres stored on a local database 
Database Title - Streaming_DB
Table Title - netflix_originals

Why was this chosen? We had a group discussion about the last Netflix movie/series we watched. This brought up the topic of different streaming services and which services provided the same movies and TV shows. We decided to narrow our findings down to Netflix originals only.
