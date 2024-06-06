# Bachelor Contestant Analysis Project

## Project Overview

This project aims to analyze data from the Bachelor TV show using the elimination week of contestants and identify the factors that contribute to a contestant's success. The project involves data cleaning, transformation, and applying machine learning models to make predictions. We train three different models: a Decision Tree Classifier, a Neural Network, and a Logistic Regression model. The Decision Tree Classifier is used to predict elimination weeks, the Neural Network is used to predict the probability of a contestant winning the season, and the Logistic Regression model is used to predict if a contestant is a winner. We also evaluate the models' performance using accuracy, confusion matrix, and other relevant metrics, visualizing the results for better understanding.


## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Contributors](#contributors)
- [Credits](#credits)

## Dataset

The datasets used in this project are sourced from the public GitHub repository of [Taylor Cox & Connor Derrick](https://github.com/tcox17/Bachelor_Project/tree/main/Original%20Datasets) and include data from 17 seasons:

- `bachelors.csv`: Information about the bachelors of each season.
- `bachelor-contestants.csv`: Information about the contestants.

## Data Preparation

The data preparation involves the following steps:

1. **Read Data**: Load the CSV files into Pandas DataFrames.
2. **Data Cleaning**:
   - Drop irrelevant columns such as height and occupation.
   - Handle missing values.
   - Change data types for consistency.
3. **Data Transformation**:
   - Split the hometown into city, state, and country.
   - Standardize state names using a dictionary of state abbreviations and full names.
   - Calculate the age difference between contestants and the bachelor.
   - Determine if a contestant is from the same state or country as the bachelor.

## Feature Engineering

Feature engineering includes:

- Encoding non-numerical values.
- Creating features such as age difference, an indicator if the contestant is younger than the bachelor, and if the contestant's home state/country matches with the bachelor.
- Creating the target variable: whether a contestant is a winner (not eliminated).

## Modeling

The modeling process involves:

1. **Decision Tree Classifier**:
   - Define features and target.
   - Split the data into training and testing sets.
   - Train the decision tree classifier.
   - Evaluate the model's performance.
2. **Neural Network**:
   - Define and compile the neural network model.
   - Train the model on the training data.
   - Evaluate the model's performance.
   - Visualize training history and predicted probabilities.
3. **Logistic Regression**:
   - Train a logistic regression classifier to predict if a contestant is a winner.

## Results

The project evaluates the models using accuracy, confusion matrix, and other relevant metrics. The results are visualized using matplotlib for better understanding.

## Contributors

- Moncia Dahl, Natasha Fidler, Anna Ramer, and Ramya Subramanian.

## Credits

The datasets used in this project are sourced from the public GitHub repository of [Taylor Cox & Connor Derrick](https://github.com/tcox17/Bachelor_Project/tree/main/Original%20Datasets). We acknowledge and thank them for providing this valuable data.

State name to abbreviation dictionary was sourced from [this Python recipe](https://code.activestate.com/recipes/577305-python-dictionary-of-us-states-and-territories/) by Mike Schultz. We appreciate their contribution to the project.


