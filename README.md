# Netflix-Movies-and-TV-Shows-Clustering
![Netflix-Symbol](https://github.com/user-attachments/assets/0fd170a8-0b3e-4cd9-8d59-cffe673a7ddd)

## Project Overview
The goal of this project is to analyze a dataset of TV shows and movies available on Netflix as of 2019. By leveraging Natural Language Processing (NLP) techniques and clustering algorithms, we aim to group similar content and develop a recommendation system. This system will enhance the user experience by suggesting relevant movies and TV shows, ultimately reducing subscriber churn.
Netflix, as the largest online streaming service with over 200 million subscribers, constantly improves its recommendations to retain users. This project contributes to that goal by identifying content clusters and improving personalization.

### Data Preprocessing
To ensure data quality and meaningful insights, we performed several preprocessing steps:

* Handling Missing Values: Missing values in key columns such as director, cast, country, and rating were addressed.

* Processing Nested Attributes: The listed_in (genre), director, cast, and country columns were tokenized and cleaned for NLP analysis.

* Binning Ratings: The rating attribute was categorized into meaningful groups such as Adult, Children, Family-friendly, and Not Rated, aiding in targeted recommendations.

### Exploratory Data Analysis (EDA)

* EDA was conducted to understand content distribution, trends, and relationships within the dataset. Key analyses included:

* Distribution of movies vs. TV shows

* Most common genres and directors

* Content availability by country

* Trends in content release over the years

These insights helped shape feature engineering for clustering.

### Clustering Approach
 * To create meaningful clusters, we employed NLP and machine learning techniques:

* Text Vectorization:

* TF-IDF Vectorizer was applied to categorical and textual attributes (director, cast, country, genre, rating, and description) to convert them into numerical representations.

* Dimensionality Reduction:

* Truncated SVD was used to reduce high-dimensional feature space, improving clustering efficiency.

### Clustering Algorithms Used:

* K-Means Clustering

* Agglomerative Hierarchical Clustering

### For Choosing the Optimal Number of Clusters:

* Elbow Method (Inertia-based evaluation)

* Silhouette Score (Cluster quality assessment)

* Dendrogram Analysis (Hierarchical clustering structure)

### Recommendation System
A content-based recommendation system was developed using Cosine Similarity Matrix that measures similarity between content based on clustered feature vectors.
Personalized Suggestions: The system suggests movies/TV shows based on user viewing history and content similarity.
This enhances the Netflix user experience by offering tailored recommendations.

### Conclusion
In conclusion, this project successfully analyzed the Netflix dataset of TV shows and movies using NLP techniques. By clustering the content and developing a content-based recommender system, we aimed to enhance the user experience and mitigate subscriber churn for Netflix. The findings and recommendations from this project can contribute to the continuous growth and success of Netflix in the highly competitive streaming entertainment industry.
