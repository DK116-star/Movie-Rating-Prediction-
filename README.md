Project Overview

This project builds a regression-based machine learning model to predict IMDb movie ratings using movie-related features such as genre, duration (runtime), cast information, popularity metrics, and critic scores. The goal is to demonstrate end-to-end data preprocessing, model building, and evaluation using scikit-learn.

🎯 Objectives

Load a public movie dataset (IMDb Top 1000)

Preprocess data by encoding categorical features and scaling numerical features

Build a regression model to predict IMDb ratings

Evaluate model performance using standard regression metrics

Identify the most important features influencing movie ratings

📂 Dataset

Source: IMDb Top 1000 Movies and TV Shows (Kaggle)

Target Variable: IMDB_Rating

Key Features Used:

Genre

Runtime (duration)

Certificate

Cast (Star1–Star4)

Number of votes (popularity)

Meta score

Release year

Gross earnings

🛠 Tools & Technologies

Python

Pandas, NumPy

Scikit-learn

ColumnTransformer

OneHotEncoder

StandardScaler

RandomForestRegressor

Pipeline

🔄 Workflow

Data Loading

Loaded IMDb dataset from CSV file

Data Preprocessing

Removed irrelevant text/image columns

Converted runtime from string to numeric

Handled missing values

Encoded categorical features using One-Hot Encoding

Scaled numerical features using StandardScaler

Model Building

Used Random Forest Regressor

Built a clean pipeline combining preprocessing and modeling

Model Evaluation

Split data into training and testing sets

Evaluated model using:

R² Score

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Feature Importance

Extracted top predictive features influencing IMDb ratings

📊 Model Performance
Metric	Value
R² Score	~0.38
MAE	~0.16
RMSE	~0.20

The model explains approximately 38% of the variance in IMDb ratings, which is a solid result for a real-world entertainment dataset.
