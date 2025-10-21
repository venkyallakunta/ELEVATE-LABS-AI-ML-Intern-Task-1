# ELEVATE-LABS-AI-ML-Intern-Task-1
# Step-1: Import the dataset and explore basic info (nulls, data types).
# Required Libraries: 
# import numpy as np, import pandas as pd, import matplotlib.pyplot as plt, import seaborn as sns
# Load the dataset i.e., titanic=pd.read_csv(r' ')
# Display the top five rows i.e.,(titanic.head())
# Check basic information ( titanic.info())
# Checking for missing values (titanic.isna().sum())
# Summary statistics (titanic.describe())
# Step-2:  Handle missing values using mean/median/imputation
# titanic['Age'] = titanic['Age'].fillna(titanic['Age'].mean()) Handle missing values in the 'Age' Column (Using Mean)
# Handle missing values in the 'Embarked' Column (Using mode Imputation)
# mode_value = titanic['Embarked'].mode()[0]
# titanic['Embarked'] = titanic['Embarked'].fillna(mode_value)
# Verify missing values are handled i.e., (print(titanic.isna().sum())
# Step- 3: Convert categorical features into numerical using encoding
# Display the updated columns i.e., ( print(titanic.columns))
# Identify and Encode Categorical Columns Dynamically 
# # Check which columns exist
# cols_to_encode = [col for col in ['Sex', 'Embarked'] if col in titanic.columns]
# if cols_to_encode:
#    titanic = pd.get_dummies(titanic, columns=cols_to_encode, drop_first=True)
# print(titanic.head())
# Check if the Column Exists Before Encoding
# print('Embarked' in titanic.columns)
# Step-4: Normalize/standardize the numerical features.
# Applying standardization using scalar
# Step-5: Visualize outliers using boxplots and remove them
# Visualize Outliers using Boxplots
