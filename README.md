# Recipe Recommender System

**Introduction**

Food.com is a popular recipe-sharing platform where users can explore, save, and review recipes. This project focuses on designing a recommender system to suggest recipes to users based on their preferences and the recipe they are currently viewing. The recommendation engine aims to increase website user engagement by presenting relevant recipes, encouraging users to spend more time exploring the platform. Higher engagement can lead to business opportunities such as collaborations, promotions, and increased revenue.
Building a recommender system from scratch can be time-consuming. In this project, we explored data and created features to develop a feature-rich recommendation engine using PySpark on an AWS EMR cluster.

**Project Overview**

**Objective**

Develop a robust recommendation system to suggest recipes to users based on their preferences and viewing history.

**Implementation Steps**

1. Data Collection
    * Utilized two datasets from S3: RAW_recipes.csv and RAW_interactions.csv.
2. Feature Engineering
    * Extracted and standardized nutritional values from the nutrition column.
    * Converted the tags column into an array format.
    * Merged interaction data with recipe data for comprehensive analysis.
    * Created time-based features, such as the difference between review dates and recipe submission dates.
    * Processed numerical columns into categorical buckets and evaluated their correlation with ratings.
    * Developed user-level features (e.g., average ratings, preparation times) to capture user preferences.
    * Extracted tag-level features to analyze tag frequencies and patterns.
3. Tools and Technologies
    * AWS EMR Cluster: For scalable distributed data processing.
    * PySpark: For efficient data manipulation and feature extraction.
    * Jupyter Notebook: For interactive development and analysis.
4. Data Storage
    * Processed data was saved in Parquet format for optimized storage and retrieval.

**Results and Conclusion**

* Outcome: The recommendation engine successfully utilized user interaction data and recipe features to generate personalized recipe suggestions.
* Insights:
    * Recipes with high nutritional balance and user ratings were more likely to be recommended.
    * User-level features provided significant improvements in recommendation accuracy.

**Recommendations**

* Leverage advanced ML models, such as collaborative filtering or neural networks, for further optimization.
* Incorporate real-time user behavior to dynamically update recommendations.
* Expand feature set by integrating external data, such as seasonal trends or regional preferences.
