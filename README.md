# project2-peloton-ETL
Project 2 and ETL: PELOTON Dataset

# Introduction
For our project, we decided to use Kaggle data from Peloton, a widely known fitness tech company. Peloton's impact includes a fitness platform of over 5.4 million members (as of June 2021) and high user satisfaction. Survey data demonstrated that 60% of users reported they were extremely satisfied with their membership and 45% would recommend the platform to family and friends. Between 2020 and 2021, Peloton grew its revenue from $1.8 billion to $38.35 billion. 

The final database produced serves a wide audience, from those working at Peloton who are interested in analyzing data on workouts or instructors to those interested in creating custom workout plans for themselves. It would also serve the journalism industry, for journalists looking to write comprehensive reports or entertainment articles on Peloton workouts. 

# Methods
In order to produce the final database in SQLite, it involved various sets of code to clean the data, joining data from two datasets, filtering the data for most desired information and finally, loading the data into the SQLite database for storage. We used two separate datasets, one with Peloton instructor info and one with Peloton workout info. This data was reported in Kaggle to be updated weekly. The instructor dataset originally had 38 columns and 58 rows, one for each instructor. The workouts dataset had 73 columns and 9,500 rows. After careful consideration of the data that the end user would want to work with, related to the introduction above, we were able to clean the two datasets and after merging produced a dataset of 11 columns.

First we cleaned each dataset separately before joining. Data cleaning involved removing unwanted columns, removing non-English characters, separating multiple data points contained in one column to two columns, renaming columns and reordering the arrangement of the columns. Then we merged the two datasets based on instructor ID in order to sort the final database by instructor name. The workout dataset contained instructor IDs (numerical values with letters) but the instructor dataset was where the full names were located. Then, the final dataset was uploaded into SQLite to produce the database shown in class. 

# Conclusion
In conclusion, we were able to produce a comprehensive database on Peloton data so that end users could query workouts based on factors important to the Peloton community, such as instructor, class duration, class description, whether music contains explicit lyrics, focus areas of the body targeted by the workouts and more. In a future project, it is possible to have kept the two datasets separate, create two separate databases, in order for the end user to have more flexibility at managing the data. 


# Reference
https://www.kaggle.com/datasets/rugbyrne/peloton 
