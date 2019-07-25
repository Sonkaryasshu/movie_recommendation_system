# Movie Recommendation System

This system recommends movie(s) based on the user's input i.e. previous movie user liked. It uses a famous algorith *Collaborative Filtering* to recommend the movies. 

## Collaborative Filtering

Collaborative Filtering simply put uses the "wisdom of the crowd" to recommend items.
Item based collaborative filtering uses the patterns of users who liked the same movie as me to recommend me a movie (users who liked the movie that I like, also liked these other movies).
Recommendation based on user's input of any movie present in the dataset.

## About dataset
I have used the MovieLens dataset and build a model to recommend movies to the end users. This data has been collected by the GroupLens Research Project at the University of Minnesota. The dataset can be downloaded from [here](https://grouplens.org/datasets/movielens/100k/) although it is available with this project in data folder. This dataset consists of:

- 100,000 ratings (1-5) from 943 users on 1682 movies
- Demographic information of the users (age, gender, occupation, etc.)

## Requirements:
- numpy
- pandas
- scipy
- sklearn


## Steps to run it on your system:

**Note:**
I am using Ubuntu 18.04 with anaconda environment and python-3.6.8


**1:** Get this project to your local system


**2:** Change directory to current project
>cd movie_recommendation_system


**3:** Recommended step *[Optional]*: Create virtual environment - Using conda here( You may use python venv)

Use the terminal or an Anaconda Prompt for the following steps:
> conda create -n myenv python=3.6 numpy pandas scipy sklearn

Activate the new environment: 
> conda activate myenv


**4:** Run the app.py file
> python main.py

**Note:** If you have created a virtual environment , you may leave it by running
> conda deactivate

### Interface
- User enters his favourite movie (or the movie on the basis of which he wants the system to recommend movies)
- Based on the user's input, recommendation is made by sorting the similarities in descending order
