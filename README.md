# Data Collection and Processing with Python Final Course Project
This is the final project in the third course of the Python 3 Programming specialisation from the University of Michigan offered through Coursera.
## About the project
This project will take you through the process of mashing up data from two different APIs to make movie recommendations. The TasteDive API lets you provide a movie (or bands, TV shows, etc.) as a query input, and returns a set of related items. The OMDB API lets you provide a movie title as a query input and get back data about the movie, including scores from various review sites (Rotten Tomatoes, IMDB, etc.).

You will put those two together. You will use TasteDive to get related movies for a whole list of titles. You’ll combine the resulting lists of related movies, and sort them according to their Rotten Tomatoes scores (which will require making API calls to the OMDB API.).
## Functions derived
### get_movies_from_tastedive
It should take one input parameter, a string that is the name of a movie or music artist. The function should return the 5 TasteDive results that are associated with that string; be sure to only get movies, not other kinds of media. It will be a python dictionary with just one key, ‘Similar’.
### extract_movie_titles
Write a function that extracts just the list of movie titles from a dictionary returned by *get_movies_from_tastedive*
### get_related_titles
It takes a list of movie titles as input. It gets five related movies for each from TasteDive, extracts the titles for all of them, and combines them all into a single list.
### get_movie_data
It takes in one parameter which is a string that should represent the title of a movie you want to search. The function should return a dictionary with information about that movie.
