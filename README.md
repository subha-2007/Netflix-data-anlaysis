# 📌 Overview

This project focuses on cleaning a raw Netflix dataset sourced from Kaggle. The raw data contained several quality issues — including a large number of null values and mixed data types within a single column — which needed to be addressed before any meaningful analysis could be performed.

All data cleaning was carried out in Google Colab using Python and the Pandas library.

## 📂 Dataset
Source: Kaggle
Description: The dataset contains information about Netflix titles (movies and TV shows), including attributes like title, director, cast, country, date added, release year, rating, and duration.
## 🧹 Data Cleaning Steps
1. Handling Null Values
Started by checking the dataset for missing values to identify which columns were affected and how severely.
Used the isnull().sum() function to get a count of missing values per column.
Filled the missing values using the fillna() function, so the dataset would no longer contain gaps that could disrupt analysis.
2. Handling Mixed Data Types
The duration column had inconsistent data — some rows represented duration in seasons (e.g., "2 Seasons") while others represented duration in minutes (e.g., "90 min").
Since a single column can't cleanly hold two different units of measurement, it was split into two separate columns:
One column to store the number of seasons (for TV shows).
One column to store the duration in minutes (for movies).
This made the data consistent and much easier to filter, sort, and analyze.
## 🛠️ Tools & Technologies
Google Colab — development environment
Python — programming language
Pandas — data cleaning and manipulation
## 🚀 Future Work
Perform exploratory data analysis (EDA) on the cleaned dataset.
Create visualizations to uncover trends (e.g., content added by year, most common genres, ratings distribution).
Build a dashboard to present key insights.


This project is for educational purposes. Dataset rights belong to the original Kaggle contributor.
