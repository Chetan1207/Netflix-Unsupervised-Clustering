# Netflix-Unsupervised-Clustering
This project's goal is to do a cluster analysis on a Netflix dataset to identify trends and group items that are similar. Information on films, actors, directors, genres, and countries was included in the collection.

The project took a methodical approach to cluster analysis:

Data Preprocessing: To manage missing values, eliminate irrelevant columns, and convert category variables into numerical representations, the dataset was cleaned and preprocessed. Text data was also processed by eliminating stopwords and tokenizing them.
Feature Extraction: Term Frequency-Inverse Document Frequency (TF-IDF) was used to vectorize text data in order to turn textual information into numerical characteristics that could be utilized for clustering.
Dimensionality Reduction: To minimize the dimensionality of the feature space while keeping significant information, Principal Component Analysis (PCA) was used. This stage aided in successfully visualizing and grouping the data.
Clustering Algorithm Selection: We explored a number of clustering techniques, including K-means and agglomerative clustering. The total number of clusters was calculated using assessment measures including the Davies-Bouldin Score, Calinski-Harabasz Score, and Silhouette Score. The best clustering method hyperparameters were discovered using GridSearchCV.
Cluster Visualization: Scatter plots, word clouds, and 3D plots were used to visualize the clusters. These visualizations aided in comprehending the clusters' properties and distributions.
Evaluation: The quality of the clusters was evaluated using evaluation measures such as the silhouette score, Calinski-Harabasz score, and Davies-Bouldin score. These measures gave us information about the clusters' separation, compactness, and similarity.
Netflix's cluster project yielded valuable insights into its dataset, uncovering hidden patterns and grouping similar items. The analysis enabled personalized recommendations, targeted marketing, and content classification. Further refinement and exploration of algorithms, parameters, and features are needed to improve clustering performance and provide a foundation for data-driven decision-making in the entertainment industry.

## CONCLUSION FROM EDA:
Netflix has more movies than TV shows available on the platform.
Love, Christmas, man, story, and world are some of the most prevalent terms used in Netflix movie descriptions, according to the Wordcloud visualization of movie descriptions.
While 95.7% of directors are connected to films, only 4.3% are connected to TV shows. Jay Karas, Marcus Raboy, Jan Suter, and Raul Campus are the leading directors.
Anupam Kher, Shahrukh Khan, and Om Puri are frequently featured actors.
The United States, India, and the United Kingdom create 51% of the total content.
The most material was released in 2019, with the most films and TV episodes released in December.
The majority of Netflix content is appropriate for mature audiences, with a TV-MA rating being the most popular. Approximately half of the shows on Netflix are produced for adult audiences.
There is a significant increase in content release from 2010 to 2020.
The most films, 1120, were released in 2018, and the most TV shows, 457, were released in 2020.
Maximum programming is composed of content lasting less than 120 minutes.

## CONCLUSION FROM MODEL IMPLEMENTATION:
The data is clustered based on the attributes: director, cast, country, genre, rating, and description.
The TFIDF vectorizer was used to tokenize, preprocess, and vectorize the data in these attributes.
The data's dimensionality, which formed the majority of the variation, was reduced using Principal Component Analysis (PCA).
The K-Means Clustering algorithm was used to create clusters, with 9 being the optimum number based on the elbow technique and Silhouette score analysis.
The agglomerative clustering technique was used to create clusters, with the dendrogram visualization indicating that 2 clusters were optimum.
Hierarchical Clustering has a better overall performance.
