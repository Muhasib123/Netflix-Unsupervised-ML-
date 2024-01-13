# Netflix-Unsupervised-ML-
Introduction:

This project delves into a dataset from 2019, sourced from Flixable, highlighting the evolution of Netflix's content landscape. Notably, a 2018 report reveals a tripling of TV shows while movies decrease by over 2,000 titles since 2010. The objective is to perform Exploratory Data Analysis (EDA), understanding content availability across countries, assessing Netflix's focus on TV versus movies, and employing clustering for text-based feature analysis.

Main Analyses:

The EDA dissects the dataset, presenting insights into the distribution of TV shows and movies, genre prevalence, and temporal trends. Concurrently, a global perspective is gained by scrutinizing content availability across different countries, identifying regional preferences and disparities. The dataset's temporal dimension is leveraged to assess whether Netflix's content strategy has shifted towards TV shows over movies.

Advanced Analysis and Conclusion:

Integration with external datasets like IMDB ratings and Rotten Tomatoes enriches the analysis, offering a comprehensive understanding of content quality and reception. Finally, text-based features are used for clustering, revealing patterns and connections beyond traditional genre classifications. This project not only contributes to decoding Netflix's content strategy but also showcases the power of data integration and advanced analytics in extracting meaningful insights from complex datasets.

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

In this project, we are required to do

Exploratory Data Analysis

Understanding what type content is available in different countries

If Netflix has been increasingly focusing on TV rather than movies in recent years.

Clustering similar content by matching text-based features.

In this project, we worked on a text clustering problem wherein we had to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.

The dataset contained about 7787 records, and 11 attributes. We began by dealing with the dataset's missing values and doing exploratory data analysis (EDA).

It was found that Netflix hosts more movies than TV shows on its platform, and the total number of shows added on Netflix is growing exponentially. Also, majority of the shows were produced in the United States, and the majority of the shows on Netflix were created for adults and young adults age group.

It was decided to cluster the data based on the attributes: director, cast, country, genre, and description. The values in these attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

We first built clusters using the k-means clustering algorithm, and the optimal number of clusters came out to be 3. This was obtained through the elbow method and Silhouette score analysis. Then clusters were built using the Agglomerative clustering algorithm, and the optimal number of clusters came out to be 9. This was obtained after visualizing the dendrogram.

A content based recommender system was built using the similarity matrix obtained after using cosine similarity. This recommender system will make 10 recommendations to the user based on the type of show they watched.
