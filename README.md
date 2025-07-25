# Flightdata_Analysis

you can the download the dataset[Google Drive]https://drive.google.com/file/d/1wPHJPLohIMmeV_55qJFpW2_EcUgWgw6c/view?usp=sharing

This project involves analyzing and classifying flight data to predict whether a flight is Long (distance > 800 miles) or Short (≤ 800 miles) based on features like fare, passenger count, and flight routes using a Logistic Regression model.
The main goal is to build a classification model that predicts if a flight is a Long Flight or a Short Flight using features such as:
Market distance
Market fare
Number of passengers
Origin and destination airports
Ticket carrier code
This binary classification problem is solved using Logistic Regression, and class imbalance is handled with SMOTE.

key steps
1.Data Preprocessing:
Handled missing values using median/zero imputation.
Dropped rows with critical missing fields (ORIGIN, DEST, TICKET_CARRIER).
Feature engineered a new binary target variable Long_Flight.

2.Feature Engineering
Created binary classification label:
Long_Flight = 1 if MARKET_DISTANCE > 800, else 0
Selected relevant features for modeling.

3. Model Training
Performed train-test split (80%-20%).
Scaled numerical features using StandardScaler.
Applied one-hot encoding on categorical features.
Used SMOTE to balance the classes in training data.
Trained a Logistic Regression model (multi_class='ovr', lbfgs solver).

5. Evaluation
Achieved training and test accuracy scores.
Visualized results with a confusion matrix.
Evaluated average market fare for short vs. long flights using bar plots.

Visual Insights
Confusion Matrix to visualize classification performance.
Bar Chart comparing average market fare for long vs. short flights.
