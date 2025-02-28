# Task-4: RECOMMENDATION SYSTEM

The Python code uses content-based filtering to recommend movies based on their descriptions.

IMPORTS :

1) pandas for data manipulation.

2) TfidfVectorizer from sklearn for text vectorization.

3) linear_kernel from sklearn for calculating cosine similarity.

4) random for generating random numbers.

DATASET :

The code reads a sample movie dataset from a CSV file using pd.read_csv.

TF-IDF VECTORIZATION :

The TfidfVectorizer is initialized with English stop words to convert the movie descriptions into a matrix of TF-IDF features (tfidf_matrix).

COSINE SIMILARITY :

The cosine similarity of the TF-IDF matrix is calculated using linear_kernel to measure the similarity between movies.

RECOMMENDATION FUNCTION :

get_content_based_recommendations(title, num_recommendations):

1) Finds the index of the given movie title.

2) Calculates similarity scores for all movies with respect to the given movie.

3) Sorts the similarity scores in descending order.

4) Selects the top num_recommendations most similar movies (excluding the given movie itself).

5) Returns the titles of the recommended movies.

RANDOM SELECTION :

A random number of recommendations (num_recommendations) is chosen between 1 and 35.

A random movie title (movie_title) is selected from the dataset.

GET RECOMMENDATIONS :

The get_content_based_recommendations function is called with the randomly selected movie title and number of recommendations.

Finally,The recommended movie titles are printed.
