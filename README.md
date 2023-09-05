# Netflix_Movies_and_TV_Shows_Clustering

![WhatsApp Image 2023-08-31 at 12 07 26](https://github.com/ShriyaChouhan/Netflix_Movies_and_TV_Shows_Clustering/assets/128309746/1dd6d65c-464c-401d-83f4-f2e810fd0591)


## Introduction:
_____________________________________________________________________________
With more than 83 million subscribers and presence in more than 190 countries, Netflix is the most popular Internet television network in the world. Its users watch more than 125 million hours of TV and movie content daily, including original series, documentaries, and feature films. On almost any screen that is linked to the Internet, members can watch as much as they want, whenever and wherever. Without interruptions or obligations, members can play, pause, and resume watching at any time.

## Problem Statement
_________________________________________________________
* Netflix is the world's largest online streaming service provider, with over 220 million subscribers as of 2022-Q2. It is crucial that they effectively cluster the shows that are hosted on their platform in order to enhance the user experience, thereby preventing subscriber churn.
* We will be able to understand the shows that are similar to and different from one another by creating clusters, which may be leveraged to offer the consumers personalized show suggestions depending on their preferences.
* The goal of this project is to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

## Project Summary
______________________________________________________
Dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

In this project, we worked on a text clustering problem where we had to classify/group the Netflix movie/shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

## Input Files:
_________________________
NETFLIX MOVIES AND TV SHOW CLUSTERING.csv

## Variables Description
__________________________________________________
The variable description of the Netflix Movies and TV Shows Clustering Dataset is as follows:
1. **show_id**: Unique identifier for each movie/show.
2. **type**: Indicates whether the entry is a movie or a TV show.
3. **title**: Name of the movie or TV show.
4. **director**: Name of the director(s) of the movie or TV show.
5. **cast**: Names of the actors and actresses featured in the movie or TV show.
6. **country**: Country or countries where the movie or TV show was produced.
7. **date_added**: Date when the movie or TV show was added to Netflix.
8. **release_year**: Year when the movie or TV show was released.
9. **rating**: TV rating or movie rating of the movie or TV show.
10. **duration**: Length of the movie or TV show in minutes or seasons.
11. **listed_in**: Categories or genres of the movie or TV show.
12. **description**: Brief synopsis or summary of the movie or TV show.

## The project follows a step-by-step process, as outlined below:---
## 1. Handling Missing Values:
      Address any null or missing values present in the dataset.
## 2. Dealing with Nested Columns:
      Process nested columns such as director, cast, listed_in, and country to facilitate clear visualization and analysis.
## 3. Rating Binning:
      Categorize ratings into appropriate categories, including adult, children's, family-friendly, and not rated content.
## 4. Exploratory Data Analysis (EDA):
      Perform in-depth EDA on various attributes, uncovering valuable findings to aid in churn prevention.
## 5. Cluster Creation: 
      Create clusters using attributes such as director, cast, country, genre, rating, and description. 
      Tokenize, preprocess, and vectorize the attribute values using TF-IDF vectorizer.
## 6. Clustering Algorithms: 
      Employ K-Means Clustering and Agglomerative Hierarchical Clustering algorithms to construct two distinct types of clusters. 
      Determine the optimal number of clusters using methods like the Elbow method and Dendrogram.

## Project Structure
________________________________________________________
## 1. README.md

## 2. Dataset 

## 3. NETFLIX MOVIES AND TV SHOWS CLUSTERING.csv

## 4. EDA

      ## Numeric & Categoric features

           # (a) Univariate Analysis

           # (b) Bivariate Analysis

           # (c) Multivariate Analysis

## 5. Data Cleaning

           # (a)  Duplicated values

           # (b)  NaN/Missing values

           # (c)  Treating Skewness

           # (d)  Treating Outlier 


## 6. Textual Data Preprocessing

          # (a) Clustering Attributes

          # (b) Removing Stopwords

          # (c) Lowercasing words

          # (d) Removing Punctuation

          # (e) Stemming

          # (f) Snowball Stemmer

          # (g) Word Vectorization

          # (h) TF-IDF (Term Frequency - Inverse Document Frequency)
 
## 7. Dimenssionality Reduction
 
          * PCA (Principle Component Analysis)


## 8.  Model Building
       # Clustering Implemention

          # (a) K-Means Clustering

          # (b) Elbow Method

          # (c) Silhoutte Score Analysis

          # (d) Agglomerative Hierarchical Clustering

              * Dendogram

## 9. Content Based Recommendation System

## 10. Future Work 

## 11. Conclusion 
In conclusion, the exploratory data analysis (EDA) of Netflix's TV shows and movies clustering has revealed a wealth of insights that shed light on the platform's content distribution, production trends, viewer preferences, and global impact. From the data, several key takeaways emerge:

## Content Diversity and Global Reach: 
Netflix's library showcases a rich diversity of content, with a focus on both TV shows and movies. The platform's international TV shows and the popularity of crime and kids' TV genres underscore the global audience's appetite for varied storytelling from different cultures and genres.

Production Trends: Over the years, Netflix has experienced rapid growth in content production. The surge in TV shows and movies from 2016 to 2020 reflects the streaming industry's evolving landscape, with platforms like Netflix responding to the demand for original content.

## Global Influences: 
The dominance of the United States in content production highlights its historical and industrial strength, while the rise of Indian content underscores the influence of factors like growing middle-class populations, disposable incomes, and the popularity of streaming services.

## Regional Success Stories: 
The prominence of South Korean dramas in the TV show market demonstrates the power of the Korean Wave, while Canada's financial support for TV shows has attracted both domestic and foreign investment.

## Viewer Engagement: 
The popularity of Japanese voice actors, crime TV shows, kids' TV, British TV shows, and documentaries showcases viewers' diverse interests, from crime thrillers to educational content, across cultures and genres.

## Quality and Collaboration:
The involvement of prolific directors and actors suggests Netflix's emphasis on quality and collaboration, both within and beyond traditional entertainment industries.

In essence, the EDA illustrates Netflix's commitment to catering to a global audience by offering diverse, engaging, and high-quality content. The platform's strategic content production, collaborations with industry leaders, and focus on viewer preferences position it as a frontrunner in the evolving world of entertainment streaming.

## Conclusions drawn from ML Model
* Implemented K-Means Clustering and Agglomerative Hierarchical Clustering, to cluster the Netflix Movies TV show dataset.
* The optimal number of clusters we are getting from K-means is 4, whereas for Agglomerative Hierarchical Clustering the optimal number of clusters are found out to be 2.
* We chose Silhouette Score as the evaluation metric over distortion score because it provides a more intuitive and interpretable result. Also Silhouette score is less sensitive to the shape of the clusters.
* Built a Recommendation system that can help Netflix improve user experience and reduce subscriber churn by providing personalized recommendations to users based on their similarity scores.
 ____________________________________________________________________________
