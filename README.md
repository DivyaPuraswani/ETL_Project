# ETL_Project
ETL_Project_Online Tutorials Data

I used 2 different datasets of popular online tutorials from the public platform Kaggle The data in the three files included the following information:
•	Udemy’s Courses
•	Coursera’s Courses

The fields of interest include the following:
•	course_id
•	course_title
•	course_students_enrolled
•	course_rating
•	course_difficulty

The following sources for our datasets used:
https://www.kaggle.com/siddharthm1698/comments

https://www.kaggle.com/andrewmvd/udemy-courses/data

#Transformation

In order to transform the public data and use it in my study I performed the following:
•	Used Pandas functions in Jupyter Notebook to load all two CSV files.
•	Reviewed the files and transformed into data frames
•	Removed the is_paid, num_lectures, course_duration, price, published_timestamp columns which was not relevant to the focus of this study when compared to columns in coursera dataframe columns.
•	Renamed the columns.
•	Due to mismatch in number of records, ie coursera having less and udemy having more randomly choose records from udemy dataframe to match number in coursera records.
•	Replaced values of 91k to 91000 i.e converting object datatype to float.
•	Created queries to find number of students enrolled in different difficulty levels, which course title has maximum number of students enrolled

#Load

The last step was to transfer my merged data into a Database. I created a database and respective table to match the columns from the final Panda's Data Frame using Postgres database using PG admin to store my original clean data sets. I reconnected to the database and generated additional tables for the data frames.

#Summary

There were some limitations to my findings due to the data available. However, I was  able to learn how to install postgres on mac, transform and load data from jupyter notebook to database and vice versa.

