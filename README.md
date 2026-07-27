# CSE 475 Final Project
CSE 475 - Introduction to Machine Learning
Final Project with Dr. Robert Atkinson
Objective: Select a "real-world" database, conduct thorough analysis, build a machine learning model(s) and "address ethical considerations related to data usage". I took a ____ sized database and trained a Naive-Bayes machine learning model to classify a movie's TV rating (G, PG, PG-13, R, NC-17, NR) based on its description, director, duration, and cast.

Please note that a lot of the text elements in my Jupyter notebooks contain "past Madeleinne voicing her thoughts out loud as she does the project". It will give myself and whoever views this an opportunity to see my thought processes, why I chose the Naive-Bayes model over other ML model types, and what I learned after each step in the project.

## Milestone 1: Analyze the Data
List of features:
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

## Milestone 2: Train the Naive-Bayes Model
At this point, I have cut down the database to 5188 rows x 16 columns. 
## Milestone 3: Test the Naive-Bayes Model
