# Netflix_Movies_and-_TV_Shows_Clustering
Introduction:
With more than 83 million subscribers and presence in more than 190 countries, Netflix is the most popular Internet television network in the world. Its users watch more than 125 million hours of TV and movie content daily, including original series, documentaries, and feature films. On almost any screen that is linked to the Internet, members can watch as much as they want, whenever and wherever. Without interruptions or obligations, members can play, pause, and resume watching at any time.

Problem statement:
Netflix has a huge selection of films and TV series, making it one of the biggest streaming services globally. It might be difficult for people to locate content that suits their interests, though, because there are so many possibilities available.

To overcome this issue, this project intends to employ unsupervised learning techniques to cluster comparable movies and TV series on Netflix. We can deliver more focused recommendations to users and assist them in discovering new content they will appreciate by grouping titles with comparable features.

This project will specifically analyze a dataset of Netflix titles, which will include variables such as genre, release year, actors, and storyline summary, among others. Our goal is to find groupings of films and TV series that have similar qualities by using clustering methods like K-Means or Hierarchical clustering.

The project's ultimate goal is to develop a clustering model that can precisely classify Netflix titles according to their attributes. After that, this approach can be applied to help Netflix enhance its content discovery algorithms or provide suggestions to users.

Overview:
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

An interesting analysis was issued in 2018 indicating that since 2010, the quantity of TV series available on Netflix has almost tripled. Since 2010, the number of movies available on the streaming service has dropped by over 2,000, but the number of TV series has increased by about three times. Investigating what further insights might be obtained from the same dataset will be interesting.

I begin by understanding the dataset and then go through and clean the data in preparation for analysis.

Investigate the data and comprehend its behavior.

Next, using a variety of factors, I have prepared the dataset for cluster creation. By doing so, I can exclude stop words, white space, and other irrelevant terms to obtain significant words, which I will then use to create clusters.

Later, I developed a recommender system using cosine similarity and suggested the top ten movies using the silhouette and k-means elbow methods to determine the ideal number of clusters.

Conclusion:
CONCLUSION FROM EDA:

Netflix offers a greater selection of movies than television series.

Most of the content on Netflix has a TV-MA rating, meaning that it is appropriate for mature audiences.

The United States leads India and the United Kingdom in the quantity of productions that are available on Netflix.

Dramas are the most popular genre on Netflix, with comedies and documentaries coming in second and third.

Love, family, youth, life, and world are among the most often used terms in Netflix movie descriptions, according to the Wordcloud visualization of movie descriptions.

The correlation heatmap demonstrates a somewhat favorable association between a film's runtime and the year of release.

The pairplot displays numerous intriguing relationships between the variables, including a negative correlation between a movie's runtime and rating and a substantial positive correlation between the number of reviews and the year of release.

CONCLUSION FROM MODEL IMPLEMENTATION:

The attributes of director, cast, nation, genre, rating, and description were used to cluster the data.

After preprocessing, tokenizing, and vectorizing the values of these attributes with TFIDF vectorizer, a total of 10,000 attributes were produced.

In order to minimize the dimensionality of the data and capture more than 95% of the variance, Principal Component Analysis (PCA) was employed.

Based on the elbow technique and Silhouette score analysis, the ideal number of clusters to be created using the K-Means Clustering algorithm was 5.

Based on the dendrogram visualization, the agglomerative clustering technique was utilized to create clusters, with five being the ideal number.

Cosine similarity was used to create a content-based recommender system that will provide the user with ten suggestions based on the kind of show they watch
