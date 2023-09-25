**Overview**
This Python program is a simple movie recommendation system that suggests movies based on their textual descriptions (overviews). It uses the TF-IDF (Term Frequency-Inverse Document Frequency) technique and the sigmoid kernel to measure similarity between movies.


**Requirements**
Python 3.x
Pandas
NumPy
Scikit-Learn


**Usage**
Data Preparation: The program assumes you have two CSV files, "tmdb_5000_credits.csv" and "tmdb_5000_movies.csv," containing information about movie credits and movie details, respectively. Make sure these files are in the same directory as the program.

Running the Program: Execute the Python script to load the data, preprocess it, and calculate similarity scores between movies. Here's how you can do it:
python movie_recommendation.py


Getting Recommendations: To get movie recommendations, you can call the give_recomendations function with a movie title as an argument. For example:
recommendations = give_recomendations('Titanic')
print(recommendations)
This will print a list of movie titles that are similar to the input movie title based on the calculated similarity scores.


**Program Components**
Data Loading and Preprocessing: The program loads movie data from CSV files, preprocesses it by cleaning and transforming the text data using TF-IDF vectorization.

Similarity Calculation: It uses the sigmoid kernel to calculate pairwise similarity scores between movies based on their TF-IDF representations.

Recommendation Function: The give_recomendations function takes a movie title as input, retrieves the most similar movies, and returns a list of recommended movie titles.


**Customization**
You can customize the program by changing parameters such as min_df, max_features, and ngram_range in the TF-IDF vectorizer to fine-tune the recommendation results.

You can also modify the number of recommended movies returned by changing the number in sig_scores[1:11] to a different value.

**Credits**
This program was created by [Devanshu3].
