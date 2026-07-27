# CSE 475 Final Project
CSE 475 - Introduction to Machine Learning
Final Project with Dr. Robert Atkinson
Objective: Select a "real-world" database, conduct thorough analysis, build a machine learning model(s) and "address ethical considerations related to data usage". I took a ____ sized database and trained a Naive-Bayes machine learning model to classify a movie's TV rating (G, PG, PG-13, R, NC-17, NR) based on its description, director, duration, and cast.

Please note that a lot of the text elements in my Jupyter notebooks contain "past Madeleinne voicing her thoughts out loud as she does the project". It will give myself and whoever views this an opportunity to see my thought processes, why I chose the Naive-Bayes model over other ML model types, and what I learned after each step in the project.

## Milestone 1: Analyze the Data
Data: netflix_titles.csv -- contains information about Netflix movies and TV shows
Database Size: 6131 x 12
List of features (12):
- show_id : the unique ID for every movie / tv show
- type : "movie" or "tv show"
- title : title of the movie
- director : director of the movie
- cast : cast of the movie
- country : where the movie or show was produced
- date_added : the date it was added on Netflix
- release_year : the actual release year of the movie or tv show.
- rating : the TV rating of the movie or TV show (e.g. PG, TV-MA...)
- duration : the total duration, in minutes (movies) or number of seasons (TV shows)
- listed_in : the genre that the movie or tv show falls under (e.g. International TV Shows, Action, Documentary)
- description: a summary description of the movie or TV show

### Steps that I took to analyze the data:
- General overview : size of the database, sample 5-10 rows, find the number of unique rows (to make sure we don't keep duplicate movies/tv shows)
- Used Histograms and Count Plots to view the distribution of movies and shows
     - Example: There are also a lot more TV-MA shows than I thought. I've always assumed that Netflix liked to cater to families, being a previously "shareable" platform and all, but there are 50% more TV-MA shows than TV-14, and the number of rated R movies is double than that of PG movies.
- I also used boxplots and violin charts to view the range of data.
- Visualized missing values with a heatmap
    - Discarded features that contain a lot of null / missing values
    - Discarded duplicate rows
- Identified outliers and anomalies using z-scores and the IQR method
    - To minimize outliers and anomalies, I capped the 'duration' feature
- Encoded features to numerically express certain features (e.g. director names, tv ratings)

## Milestone 2: Train the Naive-Bayes Model
At this point, I have cut down the database to 5188 rows x 16 columns. 
## Milestone 3: Test the Naive-Bayes Model
