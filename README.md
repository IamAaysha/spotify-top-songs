# Spotify Top 50 Songs (2021) - Data Analysis

## Overview
This project analyzes the top 50 songs on Spotify in 2021 using SQL. The dataset, sourced from Kaggle, contains song-related metadata such as key, mode, popularity, and ranking. The analysis focuses on identifying key distributions and ranking them by popularity using SQL queries in SQLite.

## Dataset
- **Source:** [Spotify Top 50 Songs (2021) - Kaggle](https://www.kaggle.com/datasets/equinxx/spotify-top-50-songs-in-2021)
- **Contains:** Song metadata including key, mode, and popularity
- **Database:** SQLite 3

## Features
### 1. **Key Identification using Pitch-Class Notation**
- The dataset uses pitch-class notation to determine the musical key of each song.
- SQL queries classify each song’s key into major or minor modes.
- Songs are grouped by key, and the total number of songs in each key is counted and sorted in descending order.

### 2. **Ranking Keys by Popularity**
- A new table (`popular_song_keys`) is created to store rankings of song keys based on music theory sources.
- Keys are assigned popularity ranks to analyze trends.

## SQL Queries & Functionality
### **Key Distribution Analysis**
- Uses `WITH` clause to classify songs into specific keys (e.g., C Major, G Minor, etc.).
- Groups and counts songs based on their musical key.
- Orders keys based on their frequency in the dataset.

### **Ranking Keys by Popularity**
- Creates a table `popular_song_keys` to store the ranking of song keys.
- Inserts values for the most to least popular keys based on music theory research.

## Insights
- Determines the most common song keys among the top 50 Spotify songs in 2021.
- Compares song key popularity against external rankings to see how industry trends align with theoretical expectations.

## Technologies Used
- **Database:** SQLite 3
- **SQL Techniques:** CTEs (`WITH` clause), `JOIN`, `GROUP BY`, `ORDER BY`, `INSERT INTO`, `CREATE TABLE`

## Potential Improvements
- Extend the dataset to include more years for a comparative trend analysis.
- Analyze correlations between song key, tempo, and popularity.
- Explore additional music features like loudness and energy levels.

## Conclusion
This project showcases how SQL can be used for analyzing music trends and metadata. By structuring data using music theory concepts, we can extract meaningful insights into the characteristics of popular songs on Spotify.

