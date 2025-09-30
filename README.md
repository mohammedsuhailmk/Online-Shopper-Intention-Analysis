# Online-Shopper-Intention-Analysis
ML program designed to predict whether a user will generate revenue (make a purchase) on an e-commerce site, based on their browsing behavior. It uses the Online Shoppers Purchasing Intention Dataset.

## Objective
The primary objective of this project is to develop a machine learning model that can predict whether an online shopper will generate revenue (i.e., make a purchase) based on their browsing behavior and session characteristics.

##  Dataset Information
    Source: UCI Machine Learning Repository
    Dataset Name: Online Shoppers Purchasing Intention Dataset
    Observations: ~12,330 rows
    Features: 17 attributes
    Target: Revenue (Boolean: True = purchase, False = no purchase)
    
   ** Categorical Features:**
        Month: Month of the session (e.g., 'Nov')
        VisitorType: New, Returning, or Other
        Weekend: Whether the session was on the weekend

## Goals
    Load and preprocess the Online Shoppers Intention dataset.

    Perform exploratory data analysis (EDA) to understand patterns and correlations.

    Encode categorical features and scale numerical values.

    Train a Random Forest Classifier to model shopper behavior.

    Evaluate model performance using accuracy, confusion matrix, and classification report.

    Predict new customer behavior using the trained model.


## Steps :

  1)  Importing necessary libraries that support data manipulation, visualisation and machine learning
  2)  Loading and balancing the Dataset to a pandas DataFrame for further preprocessing and analysis.
  3)  Exploratory Data Analysis (EDA) - Understand column types, missing values, Check for class imbalance in the target variable, Explore distributions and summary statistics.
  4)  Data Preprocessing :
            .  Encode Categorical Variables - Machine learning models require numeric input. Label encoding converts categorical variables like VisitorType into numeric form. The Month field is also numerically mapped.
            .  Handle Missing Values - Removing rows with nulls ensures clean input for training.
            .  Feature & Target Split - Separate independent (X) and dependent (y) variables for model training.
  5) Feature Scaling - Standardizing ensures all numeric features are on the same scale, improving model performance.
  6) Train-Test Split - Split data for unbiased evaluation of model performance.
  7)  Model Training - Random Forest is robust, handles both numerical and categorical variables, and is resistant to overfitting.
  8)  Model Evaluation - Assess model performance with standard classification metrics.
  9)  Predicting New User Behavior -  Create a dictionary of feature values, Convert to DataFrame and scale numeric fields, Predict using the model. 
