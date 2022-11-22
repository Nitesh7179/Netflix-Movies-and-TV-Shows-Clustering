# Netflix-Movies-and-TV-Shows-Clustering
![image](https://user-images.githubusercontent.com/93392791/203210627-9cd27e2b-20ab-46a0-b507-a70bfc3db984.png)

## Objectives:

* Conduct Exploratory Data Analysis.

* Try understanding what type content is available in different countries.

* Check if Netflix is increasingly focusing on TV rather than movies in recent years.

* Clustering similar content by matching text-based features.

## Methods used:

* Descriptive Statistics.

* Data Visualization.

* Machine Learning.

## Libraries utilized:

* NumPy and Pandas - For dataset cleaning and analysis.

* Matplotlib, Plotly and Seaborn - For Data Visualization.

* SkLearn and nltk - For machine learning and clustering.

## Dataset used:

This dataset consists of tv shows and movies available on Netflix as of 2019.
It is collected from Flixable which is a third-party Netflix search engine.

## Attribute Information:

* show_id : Unique ID for every Movie / Tv Show

* type : Identifier - A Movie or TV Show

* title : Title of the Movie / Tv Show

* director : Director of the Movie

* cast : Actors involved in the movie / show

* country : Country where the movie / show was produced

* date_added : Date it was added on Netflix

* release_year : Actual Releaseyear of the movie / show

* rating : TV Rating of the movie / show

* duration : Total Duration - in minutes or number of seasons

* listed_in : Genere

* description: The Summary description

## Project Overview:

Netflix, is an American subscription streaming service and production company. It was founded in 1997 by Reed Hastings and Marc Randolph in Scott’s Valley, California.

It offers a library of films and television series through distribution deals as well as its own productions, known as Netflix Originals.

Our objective is to conduct an Exploratory Data Analysis to understand what content is available in different countries and if Netflix has been increasingly focusing on TV rather than movies in recent years. And use these insights to cluster similar content by matching text-based features.

After loading the data, we start by observing the first and last five values to understand the dataset. Next, we treat the null values by dropping them if the respective variables contain <1% of null values. This is followed by feature engineering to extract new variables from the datetime variable date_added.

This cleaned data is then used to conduct EDA in order to understand it better and identify the underlying trends.

Once obtained the required insights from the EDA, we start with Pre-processing the text data by removing the punctuation, and, stop words. This filtered data is passed through TF - IDF Vectorizer since we are conducting a text-based clustering and the model needs the data to be vectorized in order to predict the desired results.

Finally, K–Means clustering is utilized to form 10 distinct clusters with similar data points.

Using the data provided, we also implemented a simple recommender system that successfully generates Ten similar Movies or Tv-Shows for the given title.

## CONCLUSION:-

* From elbow and silhouette score, optimal of 26 clusters formed, K Means is best for identification than Hierarchical as the evaluation metrics also indicate the same. In kmean cluster 0 has the highest number of data points and is evenly distributed for other clusters.

* Netflix has 5372 movies and 2398 TV shows, and there are more number movies on Netflix than on TV shows.

* TV-MA has the highest number of ratings for tv shows i.e adult ratings

* Highest number of movies released in 2017 and 2018

highest number of movies released in 2020 The number of movies on Netflix is growing significantly faster than the number of TV shows. We saw a huge increase in the number of movies and television episodes after 2015. there is a significant drop in the number of movies and television episodes produced after 2020. It appears that Netflix has focused more attention on increasing Movie content than TV Shows. Movies have increased much more dramatically than TV shows

* The most content is added to Netflix from October to January

* Documentaries are the top most genre on Netflix which is followed by standup comedy and Drams and international movies

* kids tv is the top most TV show genre in Netflix

* Most of the movies have a duration of between 50 to 150

* Highest number of tv_shows consisting of single season.

* Those movies that have a rating of NC-17 have the longest average duration.

When it comes to movies having a TV-Y rating, they have the shortest runtime on average

* United states has the highest number of content on Netflix, followed by India

* India has the highest number of movies on Netflix

* 30% of movies are released on Netflix.

* 70% of movies added on Netflix were released earlier by different modes.
