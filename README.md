# Tourist Attraction Recommendation System

This project leverages user ratings and attraction data to recommend tourist spots using collaborative filtering and Singular Value Decomposition (SVD). It covers data exploration, recommendation model training, and evaluation.

## Table of Contents
1. [Project Structure](#project-structure)
   - [1. Data Exploration and Preprocessing](#1-data-exploration-and-preprocessing)
   - [2. Exploratory Data Analysis (EDA)](#2-exploratory-data-analysis-eda)
   - [3. Recommendation System Using SVD](#3-recommendation-system-using-svd)
2. [Key Insights](#key-insights)
3. [Model Performance](#model-performance)
4. [Suggestions for Improvement](#suggestions-for-improvement)
5. [Conclusion](#conclusion)
6. [Future Work](#future-work)

## Project Structure

### 1. Data Exploration and Preprocessing
The project uses three main datasets:
- `tourism_with_id.xlsx`: Contains information about tourist attractions, such as `Place_Id`, `Place_Name`, `Price`, and `Category`.
- `tourism_rating.csv`: Contains user ratings for tourist spots.
- `user.csv`: Contains user demographic data, such as `User_Id`, `Age`, and `Location`.

Data was cleaned, merged, and prepared for analysis, including handling missing values and outliers.


### 2. Exploratory Data Analysis (EDA)
EDA provided insights into user demographics, ratings distribution, and the popularity of tourist attractions.

Key Observations:
- **Age Distribution**: Most users are in their late 20s and early 30s.
- **Top Categories**: Amusement parks (`Taman Hiburan`) and cultural sites (`Budaya`) are the most popular tourist attractions.

**Screenshots**:
- Age Distribution Histogram: Showcasing the distribution of users' ages.

![AgeDistribution](https://github.com/user-attachments/assets/d988f0c0-43e9-48df-b40b-0c6c2ad614b1)

- Bar Chart of Tourist Attraction Categories: Highlighting the most popular categories of attractions.

![TouristSpotDistribution](https://github.com/user-attachments/assets/31c5bcb2-82ee-46cf-9bd1-cedce8fd154e)


### 3. Recommendation System Using SVD
The project employs collaborative filtering using SVD to predict ratings and recommend tourist spots to users.

Steps:
- **Matrix Construction**: A user-item matrix was created where rows represent users and columns represent tourist spots.
- **Singular Value Decomposition**: Applied SVD to reduce the dimensionality of the matrix.
- **Prediction and Recommendations**: Predictions were generated based on user preferences and historical data.

**Screenshots**:
- Model Performance (Root Mean Squared Error): Visualize RMSE and MAE values for model evaluation.

<img width="218" alt="ModelPerformance" src="https://github.com/user-attachments/assets/9900cff0-717f-4b35-b1cf-8eff0a724f23">


## Key Insights

- **Most Popular Categories**: Amusement parks and cultural sites dominate the tourism landscape in terms of user preferences.
- **Top Tourist Destinations**: Bandung and Yogyakarta are the most frequently visited cities with highly rated attractions.

## Model Performance

- **Collaborative Filtering with SVD**: The model achieved an RMSE of 1.41 and MAE of 1.21, indicating reasonable accuracy in predicting user preferences.

## Suggestions for Improvement
1. **Incorporate Additional Features**: Adding user engagement metrics (e.g., frequency of visits) may improve recommendations.
2. **Enhance the Dataset**: Including data on seasonal effects or special events could help provide more context to the recommendations.
3. **Optimize Model Parameters**: Further tuning of the SVD model's hyperparameters might improve the accuracy of predictions.

## Conclusion
This project demonstrates the effectiveness of collaborative filtering in recommending tourist attractions. Insights gained from EDA reveal that certain types of attractions and cities are particularly popular among users. 

## Future Work
1. **Expand the Recommendation System**: Incorporate additional factors such as user location, travel preferences, and external data (e.g., weather conditions).
2. **Improve Model Performance**: Experiment with advanced recommendation algorithms, such as neural networks or deep learning-based recommendation systems.
3. **User-Based Analysis**: Personalize recommendations further by clustering users based on demographic and behavioral data.
