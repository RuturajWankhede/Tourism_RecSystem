# Tourism Recommendation System and EDA on User Ratings

This project focuses on building a tourism recommendation system using collaborative filtering techniques and performing exploratory data analysis (EDA) on user ratings of various tourist spots. The dataset includes user demographics, place ratings, and detailed information about tourism spots such as locations, categories, and more.

## Table of Contents

- [Objective](#objective)
- [Dataset](#dataset)
- [Approach](#approach)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Setup](#setup)
- [Future Work](#future-work)
- [Contact](#contact)

## Objective

The project has two main objectives:
1. Perform detailed exploratory data analysis (EDA) on the dataset to understand the user rating patterns, popular tourist spots, and user demographics.
2. Build a recommendation system using collaborative filtering techniques to suggest tourist spots based on user ratings.

## Dataset

The dataset includes information on:
- **User Ratings**: Ratings given by users to various tourist spots.
- **Tourist Spot Information**: Name, category, location, and rating of tourist spots.
- **User Information**: User ID, age, and location.
- **Missing Data**: The dataset also contains missing values, which are handled during the analysis.

The data is stored in the following files:
- `tourism_with_id.xlsx`: Contains information on the tourist spots.
- `user.csv`: Contains user demographic data.
- `tourism_rating.csv`: Contains the ratings given by users to the tourist spots.

## Approach

### 1. Exploratory Data Analysis (EDA):
- **Tourist Spot Analysis**: We analyzed the most popular tourist spots based on ratings, locations, and categories.
- **User Demographics**: Insights into the age distribution and geographic origins of users.
- **Missing Data Handling**: Identified and handled missing values in key columns, such as the `Time_Minutes` and `Unnamed` columns.

### 2. Recommendation System:
- **Collaborative Filtering**: A user-based collaborative filtering algorithm was applied using the **SVD (Singular Value Decomposition)** technique to predict user ratings for tourist spots.
- **Evaluation**: The recommendation system was evaluated using metrics such as RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error).

### Code Highlights:
- **Data Cleaning**: Handled missing values and irrelevant columns.
- **Visualization**: Matplotlib and Seaborn were used for visualizing the distribution of ratings, popular tourist spots, and user demographics.
- **Collaborative Filtering**: Built a user-based collaborative filtering recommendation system using the **Surprise** library for Python.

## Results

- **Most Loved Tourist Spots**: The top-rated tourist spots included historical and cultural landmarks such as Keraton Surabaya and Monumen Nasional.
- **User Demographics**: The most active age groups for ratings were users in their 20s and 30s, with significant engagement from regions like Jakarta and Yogyakarta.
- **Recommendation System Performance**: Achieved a Root Mean Squared Error (RMSE) of 1.42, indicating reasonable performance for predicting user preferences.

## Technologies Used

- **Programming Languages**: Python
- **Libraries**: 
  - **Data Analysis**: Pandas, NumPy
  - **Visualization**: Matplotlib, Seaborn
  - **Machine Learning**: Scikit-learn, Surprise Library (for collaborative filtering)
  
## Setup

To get started with this project:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/tourism-recommendation-system.git
