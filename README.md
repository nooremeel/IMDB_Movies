# IMDb Movie Data Analysis

## Project Overview
This project involves analyzing IMDb movie data using **Python** for data cleaning and **Power BI** for modeling and visualization. The objective is to clean the dataset, handle missing values, and provide meaningful insights into the dataset through visualizations.

## Table of Contents
1. [Data Cleaning](#data-cleaning)
2. [Modeling and Visualization](#modeling-and-visualization)
3. [Key Insights](#key-insights)
4. [Technologies Used](#technologies-used)
5. [Getting Started](#getting-started)

## Data Cleaning

1. **Data Import:**
   - Loaded the dataset into a Pandas DataFrame.
   
2. **Data Transformation:**
   - Removed commas from the 'Gross' column and changed its data type to numeric.
   - Removed 'min' from the 'Runtime' column and changed it to numeric.
   - Corrected the release year of *Apollo 13* to '1995'.
   - Replaced null values:
     - 'Certificate' column: Replaced nulls with 'Unknown'.
     - 'Meta_score' column: Replaced nulls with 0.
     - 'Gross' column: Replaced nulls with the mean.
   - Removed whitespaces from the 'Genre' column.

## Modeling and Visualization

1. **Data Loading:**
   - Imported the cleaned dataset into Power BI.

2. **Data Modeling:**
   - Split the 'Genre' column using Power Query to handle multiple genres.
   - Created a 'Movie_ID' column by merging 'Series Title' and 'Release Year'.
   - Established a one-to-many relationship between the main table and a new genre-specific table using 'Movie_ID'.

3. **Visualizations:**
   - **Bar Chart:** Number of movies per genre.
   - **Column Chart:** Highest grossing movie of each year.
   - **Histogram:** Most popular movie runtimes.
   - **Bar Chart:** Top average ratings of directors.
   - **Line Chart:** Number of votes over the years.
   - Created a dashboard with interactive slicers for filtering.

## Key Insights
- The most frequent movie genres and their distribution.
- Highest grossing movies per year, revealing trends in box office success.
- Popular runtimes for movies and insights into average movie lengths.
- Directors with the top average ratings, showing a correlation with critical acclaim.
- Trends in the number of votes over time, reflecting audience engagement.

## Technologies Used
- **Python**: Data Cleaning (Pandas)
- **Power BI**: Data Modeling, Visualization, and Dashboard Creation
