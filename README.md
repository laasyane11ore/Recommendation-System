# Recommendation-System
Movie recommendation system using collaborative filtering and k-Nearest Neighbors (kNN). It aims to recommend similar movies to a given movie based on user ratings.
## Libraries 
* numpy: For numerical operations.
* pandas: For data manipulation and analysis.
* sklearn: For machine learning algorithms.
* matplotlib: For plotting data.
* seaborn: For visualization.
* scipy: For creating sparse matrices.
## Data 
* "https://s3-us-west-2.amazonaws.com/recommender-tutorial/ratings.csv": Contains user ratings for movies.
* "https://s3-us-west-2.amazonaws.com/recommender-tutorial/movies.csv": Contains movie details.
## Data Exploration
prints the number of ratings, the number of unique movie IDs, the number of unique users, and the average ratings per user and per movie.
<img width="220" alt="data_explore" src="https://github.com/laasyane11ore/Recommendation-System/assets/138700086/f34dbc4a-e82e-4bea-b8bd-b760a59468fb">
## Create User-Item matrix
The function create_matrix converts the ratings DataFrame into a sparse user-item matrix using scipy's csr_matrix.
## Find similar movies using KNN
The function find_similar_movies takes a movie ID and the user-item matrix and uses k-Nearest Neighbors to find similar movies.
It calculates the similarity between the given movie and other movies using the chosen metric (default is cosine similarity).
The function returns a list of similar movie IDs.
## Result/Recommendations
<img width="246" alt="movie_reccomendation" src="https://github.com/laasyane11ore/Recommendation-System/assets/138700086/f229fbfe-ab03-4e6c-8fdd-d059760f279f">

## Conclusion
This code demonstrates how to build a simple movie recommendation system using collaborative filtering and k-Nearest Neighbors. It calculates the similarity between movies based on user ratings and suggests similar movies to a given input movie.
