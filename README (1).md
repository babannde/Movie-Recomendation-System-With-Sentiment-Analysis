
# Content-Based-Movie-Recommender-System-with-sentiment-analysis-using-AJAX

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using beautifulsoup4 and performed sentiment analysis on those reviews


## Getting the API Keys
Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your API sidebar once your request is approved.



## Run Locally

Clone the project

```bash
  git clone https://github.com/babannde/Movie-Recomendation-System-With-Sentiment-Analysis/
```

Go to the project directory

```bash
  cd Movie Recomendation System With Sentiment Analysis
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)

Replace YOUR_API_KEY in both the places (line no. 15 and 29) of static/recommend.js file and hit save.

Open your terminal/command prompt from your project directory and run the file main.py by executing the command

```bash
  python main.py
```

Start the browser

```bash
  http://127.0.0.1:5000/
```


## Documentation

## Similarity Score :

## How does it decide which item is most similar to the item user likes?

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

## How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.




## Datasets

- [IMDB 5000 Movie Datasets](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
- [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
- [Movie List 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
- [Movie List 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
- [Movie List 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)


## Authors

- [@babannde](https://www.github.com/babannde)


## Acknowledgements

 - [Krish]()
 - [Kishan]()

