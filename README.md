# Hotel Data BigData Analysis

## Project Overview
This project aims to analyze hotel pricing and booking behavior using big data tools and machine learning models. By integrating data from JSON and CSV files, we gain insights into hotel characteristics, booking trends, and factors affecting pricing. The project utilizes PySpark for big data processing and machine learning algorithms to predict hotel prices and analyze booking patterns.

## Key Features
- **Data Integration**: Combines JSON and CSV datasets to form a comprehensive dataset for analysis.
- **Big Data Processing**: Uses PySpark for efficient data handling and processing.
- **Machine Learning**: Implements predictive models for price prediction and classification of hotel bookings.
- **Data Visualization**: Provides insights through various visualizations, including price distribution, correlations, and feature importance.

## Usage

## Data loading and preprocessing
Exploratory Data Analysis (EDA)
Model training and evaluation for both price prediction and hotel classification
Visualizing insights and interpreting results
Run Individual Scripts: Alternatively, you can run each script in the src folder for specific tasks. Each script is designed to be modular and can handle data processing, analysis, or model training independently.

## Data Description
Madrid.json: Contains data on various hotels, including attributes like ratings, prices, and locations.
hotel_bookings.csv: Contains booking information, such as lead time, total stay, price per person, and cancellation status.
merged_data.csv: The merged dataset from the JSON and CSV files, offering a holistic view of hotel pricing and booking patterns.

## Model Overview
We apply machine learning models to each dataset to predict prices and classify hotel types based on various features:

JSON Dataset:
Models: Random Forest, XGBoost
Target: Predict hotel prices based on star ratings, distance, and other attributes.
CSV Dataset:
Model: Logistic Regression
Target: Classify bookings as either city hotel or resort hotel.
Merged Dataset:
Model: Gradient Boosting Regressor
Target: Predict hotel prices using features from both booking details and hotel characteristics.

## Results and Findings
JSON File:

Key Features: Star ratings, rating score, and distance from the city center were the most influential factors in predicting prices.
Model Performance: Random Forest performed best, with an RMSE of 53.08 and an R² score of 0.63.
CSV File:

Key Features: Lead time, total stay, ADR (average daily rate), and price per person influenced booking type predictions.
Model Performance: Logistic Regression achieved an accuracy of 70.97%.
Merged Dataset:

Key Features: Rating score, total stay, and lead time were significant predictors of hotel prices.
Model Performance: Gradient Boosting Regressor showed the best results with an RMSE of 20.18 and an R² of 0.39.

## Tools and Technologies
Programming Language: Python
Big Data Processing: PySpark
Machine Learning: Scikit-Learn, XGBoost
Data Visualization: Matplotlib, Seaborn
Notebook Environment: Jupyter

## Big Data Processing: Hadoop vs. PySpark
This project highlights the comparison between Hadoop and PySpark for big data handling:

Hadoop: Effective for batch processing with MapReduce but has a steeper learning curve.
PySpark: More flexible and faster with in-memory processing, ideal for iterative tasks like machine learning. Chosen as the primary tool in this project for its speed and ease of use.
