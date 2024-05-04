# Movie Recommendation System

This project implements a movie recommendation system using content-based filtering. It utilizes movie metadata such as genres, keywords, cast, and crew to recommend similar movies to a given movie title.

## Introduction

The code reads movie data from two CSV files: `tmdb_5000_credits.csv` and `tmdb_5000_movies.csv`. It merges the dataframes based on the movie title and preprocesses the data by handling missing values, converting text data into usable formats, and generating tags for each movie based on its metadata. Using these tags, the code constructs a similarity matrix to find movies similar to a given movie title.

## Usage

1. Place the CSV files (`tmdb_5000_credits.csv` and `tmdb_5000_movies.csv`) in the same directory as the code.

2. Run the provided code in a Python environment that supports the necessary libraries.

3. The code preprocesses the data, constructs a movie recommendation system, and saves the necessary files (`movie_list.pkl` and `similarity.pkl`) for future use.

4. To recommend movies, load the saved files (`movie_list.pkl` and `similarity.pkl`) and use the `recommend(movie_title)` function, providing a movie title as input.

## File Description

- `movie_recommendation_system.ipynb`: Jupyter notebook containing the code for the movie recommendation system.
- `README.md`: This file providing an overview of the project.
- `tmdb_5000_credits.csv`: CSV file containing movie credits data.
- `tmdb_5000_movies.csv`: CSV file containing movie metadata.
- `movie_list.pkl`: Pickle file containing preprocessed movie data.
- `similarity.pkl`: Pickle file containing the similarity matrix for movies.

## Requirements

- Python 3.x
- pandas
- scikit-learn
- numpy

## License

This project is licensed under the MIT License.

