# Filmy - The Movie Recommender 


<div align="center"> <img align="center" alt="viraan" src="https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Filmy-%20The%20Movie%20Recommender1.jpg" height='100' width='100'> </a> </div>
<br /><br />


![Framework](https://img.shields.io/badge/Framework-Flask-red)
![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
![API](https://img.shields.io/badge/API-TMDB-fcba03)

- Filmy is a Content-Based-Movie-Recommender.

- A Content-Based Recommender works by the data that we take from the user, either explicitly (rating) or implicitly (clicking on a link). By the data we create a user profile, which is then used to suggest to the user, as the user provides more input or take more actions on the recommendation, the engine becomes more accurate.

- Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.

- The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using `beautifulsoup4` and performed sentiment analysis on those reviews.


- Hey There! If the movie that you are looking for is not auto-suggested. Just type the movie name in the search barand click on "Enter". You will be good to go eventhough if you made some typo errors.


## How to run the project?

1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/requirements.txt) file with the command `pip install -r requirements.txt`
3. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
4. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
5. Hurray! That's it.

## Architecture :

 ![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Architecture_img.png)

## Cosine Similarity used here :
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
  
  ![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/cosine_similarity.png)
## Machine learning model used:

I have incorporated machine learning models like bag of words, tf - idf vectorization, similarity analysis, and review analysis on the basis of multinomial naïve bays algorithm. Which is a Bayesian learning approach popular in Natural Language Processing (NLP).

## Similarity Score : 

   How does it decide which item is most similar to the item user likes? Here come the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
   ## Features :
   
   - The landing page is consists of a search bar where we can search any movie name it provides auto-complete feature and also provide some suggestions of movie name    whatever you type in the search bar .
- After writing any movie name click on the Enter button below of search bar.
- It will provide the movie title, movie poster, overviews, rating, genre, release date, runtime, status.

- It also provides top cast name and their details like birthday, place of birth, and biography.
- The Filmy – The movie Recommender also provides user reviews in terms of comments and sentiments that is very important for deciding any particular searched movie is good or bad.
- Now the main feature that is recommending the movie similar to that of the searched movie comes below of reviews.
- If we click any of the recommended movie poster it takes us to the page of that clicked movie .
- And once again we can see that all details for that clicked movie comes as that of previous searched movie .
   

## Note : 

Datasets of credits.csv and movies_metadata.csv download from [here](https://www.kaggle.com/rounakbanik/the-movies-dataset)
download these two datasets and put it in the same directory of downloaded/cloned folder.
  
<!-- More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/) -->
## Landing Page
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/landing_page.gif)
## Search Bar
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot1.png)
## Search Result
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot2.png)

## Top Cast
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot3.png)
## Cast and Crew
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot4.png)
## Details of Cast
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot5.png)
## User Reviews
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot6.png)
## Recommended Movies

![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot7.png)
## Recommended Movies Continue..
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot8.png)
## Recommended Movies Continue..
![Uzoma Medium Gif](https://github.com/Gourav1695/Filmy-The_Movie_Recommender/blob/main/screenshot/Screenshot9.png)

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)



## Made by 

| Name                  | Role                       | GitHub Username:octocat:                             |
| ------------------    | -------------------------- | ---------------------------------------------------- |
| Gourav Kumar Shaw     | Overall developement       | [@Gourav1695](https://github.com/Gourav1695)       |
