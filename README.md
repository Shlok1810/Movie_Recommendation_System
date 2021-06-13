Movie-Recommender-System

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB and using the IMDB id of the movie in the API, We did web scraping to get the reviews given by the user in the IMDB site using `beautifulsoup4` and performed sentiment analysis on those reviews.


## The Movie Cinema

We've developed a similar application called "The Movie Cinema" which supports all language movies. But the only thing that differs from this application is that I've used the TMDB's recommendation engine in "Movie-Recommender-System". The recommendation part developed by me and kishan in this application doesn't support for multi-language movies as it consumes 200% of RAM (even after deploying it to AWS, Heroku ) for generating Count Vectorizer matrix for all the 700,000+ movies in the TMDB. 

## How to run the project?

1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt](https://github.com/Shlok1810/Movie_Recommendation) file with the command `pip install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/.
4. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
5. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.


How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.


 Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
