# Netflix-movies-and-Tv-shows-clustering
Project Summary - The project delves into an extensive dataset sourced from Flixable, offering a comprehensive snapshot of Netflix's content library up until 2019. Noteworthy findings emerged, including a remarkable surge in TV show offerings since 2010, contrasting with a substantial drop in movie titles during the same period.

A systematic approach was adopted, commencing with a meticulous review of the dataset's structure and contents. Rigorous data cleaning procedures were then implemented, ensuring the dataset was primed for in-depth analysis. Exploratory Data Analysis (EDA) unveiled intriguing patterns, trends, and overarching behaviors within the dataset.

To facilitate clustering, a series of text preprocessing techniques were deployed, encompassing the removal of stop words, extraneous characters, and numerical values. This refinement process uncovered pivotal keywords instrumental in shaping the subsequent clusters.

Two distinct methodologies were applied to ascertain the optimal number of clusters for the analysis: the Silhouette Method and the K-Means Elbow Method. These strategies provided a robust foundation for grouping analogous TV shows and movies based on their intrinsic characteristics.

The project culminated in the development of a recommender system, leveraging cosine similarity—a potent technique measuring the likeness between items in the dataset. This empowered the system to offer tailored recommendations, suggesting the top five movies akin to a user's stated preferences.

In summary, this exhaustive analysis of the Netflix dataset yielded profound insights into the dynamic evolution of available content on the platform. The integration of clustering and the recommender system revolutionized the user experience, enabling individuals to unearth pertinent TV shows and movies in alignment with their tastes. This amalgamation of data-driven techniques not only enriched the streaming experience but also shed light on the ever-evolving landscape of content consumption in the digital age.

Problem Statement

The dataset we're investigating provides a comprehensive overview of Netflix's content library as of 2019, sourced from Flixable, a respected third-party Netflix search engine. A significant trend identified from a report in 2018 underscores a compelling narrative: the quantity of TV shows available on Netflix has nearly tripled since 2010. In stark contrast, the platform experienced a notable reduction in its movie offerings, with over 2,000 titles being removed during the same period. This dichotomy raises intriguing questions and opens up avenues for deeper exploration.

Our primary objective is to delve into this dataset with a meticulous approach. This involves rigorous data cleaning, exploratory data analysis (EDA), and text preprocessing. By doing so, we aim to unearth further fascinating patterns and trends within Netflix's extensive content library. Potential insights waiting to be discovered include identifying prevalent genres, pinpointing top-rated TV shows and movies, discerning regional viewing preferences, tracking release patterns over the years, and gauging user sentiment for different titles. These insights hold the potential to significantly influence Netflix's decision-making processes concerning content acquisition, user engagement strategies, and overall content curation.

Furthermore, we intend to leverage advanced clustering techniques, such as k-means, to group together TV shows and movies that share similar characteristics. This clustering analysis has the potential to unveil hidden patterns and preferences among the audience, which, in turn, can empower Netflix to deliver highly personalized content recommendations to its users.

In addition to clustering, we plan to construct a robust recommender system utilizing collaborative filtering or content-based filtering approaches. This system will serve to augment the user experience by suggesting TV shows and movies that align closely with individual viewing histories and preferences.

In summation, our endeavor to explore this dataset presents a distinctive opportunity to gain invaluable insights into the evolving landscape of content on Netflix. It offers a nuanced understanding of the shifting preferences of the platform's audience over the years. These insights, when appropriately harnessed, have the potential to not only optimize content curation but also enhance user satisfaction and drive strategic decisions for the streaming service.

What did you know about your dataset?

Dataset Size: The dataset contains 7787 rows and 12 columns, representing 7787 entries or records, and each entry has 12 different pieces of information.

Netflix Content Classification: The content in the dataset is classified into two main categories: "tv shows" and "movies." Each entry in the dataset is either a TV show or a movie.

Unique Show IDs: Each show has a unique identifier represented by "s1," "s2," and so on. These IDs help distinguish one show from another in the dataset.

Title, Director, and Cast Information: For each show, the dataset includes its title, providing the name of the show. Additionally, it includes information about the director(s) responsible for creating the show and the cast members who portray the characters in the show.

Sourcing Nations: Netflix sources content from 681 different nations. These nations represent the diverse origins of the content available on the platform.

Date Column: The date column provides important information about the show. It includes details on when the show was added to Netflix, helping users understand when it became available for streaming on the platform. The column also contains information on the year the show was originally released.

Rating: The rating column indicates the classification given to the show based on its content. It helps viewers decide if the show is suitable for their age group or preferences.

Listed Shows: There are 419 different types of listed shows in the dataset. These listed shows represent various genres and categories available on Netflix, such as foreign TV shows, romantic comedies, thrillers, and more.

Unique Values: In total, there are 216 unique values in the dataset, encompassing information about the show descriptions and durations. The descriptions provide additional details about the content and its storyline, while the durations represent the number of minutes in a single season of the show.

The dataset presents a comprehensive overview of Netflix's content library, including diverse shows and movies from various nations, with detailed information about their titles, directors, casts, and genres. This information enables users to explore and discover content that suits their preferences and interests.

Summary and Conclusion:

In this project, we tackled a text clustering issue where we had to categorize Netflix shows into specific clusters such that the shows within a cluster are similar to one another and the shows in different clusters are dissimilar to one another.

1. The project aimed to address a text clustering task, where the primary objective was to categorize Netflix shows into specific clusters. The goal was to group shows within a cluster that are similar to each other, based on their attributes and content, while ensuring that shows in different clusters are dissimilar.

2. During the data preprocessing stage, the dataset was checked for duplicates and missing values. Fortunately, no duplicate entries were found. However, certain columns, such as director, cast, country, and date_added, had missing values. To address this, appropriate values were used to fill in the missing entries.

3. The analysis revealed that movie shows account for 69% of Netflix's content, whereas TV shows make up 31%. This indicates that Netflix has a more extensive collection of movie content than TV shows.

4. Over the years, Netflix has been steadily adding more shows to its platform. The majority of movies were released in 2017 and 2018, while most television shows were added in 2019 and 2020. It is suggested that the decline in the number of movies added in 2020 might be attributed to the COVID-19-induced lockdowns that affected show production.

5. Netflix's focus on expanding its movie show library is evident, as it has been adding movie content at a faster rate than TV shows.

6. Seasonal patterns were observed in content releases, with more shows being released during the Christmas season (October, November, December, and January).

7. The analysis of popular categories on Netflix revealed that documentaries are the most preferred, followed by stand-up comedy, dramas, and foreign films. For TV shows, Kids TV emerged as the most well-liked category.

8. The majority of movies have durations lasting between 90 and 120 minutes, while TV shows tend to have just one season.

9. NC-17 rated movies were found to have the longest average runtimes, while TV-Y rated movies had the shortest average duration.

10. Geographical visualizations provided insights into content production, showing that the United States and India are the leading countries in terms of contributing content to Netflix.

11. For clustering the data, the attributes selected were director, cast, country, genre, and description, as these features play a significant role in defining the content of a show.

12. Tokenization, preprocessing, and vectorization using the TFIDF vectorizer resulted in 20,000 characteristics to represent the shows.

13. Principal Component Analysis (PCA) was applied to address the high dimensionality of the data and reduce it to 4,000 components while retaining over 80% of the variance. This step was crucial to efficient clustering.

14. The optimal number of clusters, six, was identified using the K-means clustering technique, employing the elbow method and Silhouette score analysis.

15. Agglomerative clustering was utilized with 12 clusters, determined as the optimum number through visualization of the dendrogram.

16. A similarity matrix obtained through cosine similarity was instrumental in constructing a content-based recommender system. This system provides personalized recommendations to users based on their previous show preferences, helping enhance user engagement.

17. Overall, the project aimed to improve user experience on Netflix by effectively categorizing shows into clusters and providing relevant recommendations. By understanding user preferences and delivering tailored content, Netflix can increase user satisfaction and retention, ultimately benefiting the platform's success.
