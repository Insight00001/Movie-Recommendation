# Movie-Recommendation
this repository contains code for recommending similar movies to users based on the kind of movie entered using cosine similarity
# DataSet
the data set used for the course was collected from Kaggle: Kaggle datasets download -d parthdande/imdb-dataset-2024-updated
#features
the dataset contains 

    Title: The name of the movie.
    IMDb Rating: The IMDb rating of the movie.
    Year: The year the movie was released.
    Certificates: The certification of the movie (e.g., R, PG-13).
    Genre: The genre(s) of the movie.
    Director: The director of the movie.
    Star Cast: The main actors in the movie.
    Metascore: The Metacritic score of the movie
    Duration (minutes): The duration of the movie in minutes.
 # Analyzing Relationship
    We'll analyze the relationships between IMDb ratings and the following features:
    Year
    Certificates
    Genre
    Director
    Metascore
    Duration (minutes)
    this bivariate analysis is performed to find the relationship between two features

# feature Engineering
relevant features were combined to form a single feature called a combined feature
Genre, director, and certificates 

# Method

First, we take the input in the get recommendation function

Then we take the index of the input and see which data matches

Then we compute a cosine similarity for this input and all the other entries in the data on the combined score

Then we sort the cosine similarity and return the top most cosine similar entries in the data (recommendations)

      
