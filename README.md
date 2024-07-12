# Titanic Survival Prediction

This project analyzes the Titanic dataset to predict survival using various machine learning classifiers. It explores relationships between different features and survival rates and implements several classification algorithms to compare their performance.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Data Description](#data-description)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

The goal of this project is to predict which passengers survived the Titanic disaster using machine learning techniques. We analyze the data, preprocess it, and build models using different classification algorithms.

## Installation

To run this project, you need to have Python installed along with the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Data Description

The dataset used in this project is `titanic_data.csv`. It contains the following columns:

- `Survived`: Survival (0 = No, 1 = Yes)
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Sex`: Sex
- `Age`: Age in years
- `SibSp`: Number of siblings / spouses aboard the Titanic
- `Parch`: Number of parents / children aboard the Titanic
- `Fare`: Passenger fare
- `Embarked`: Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

## Exploratory Data Analysis

We perform EDA to understand the data distribution and relationships between features:

- **Correlation Heatmap**: Shows correlations between features.
- **Survival Probability by SibSp**: Analyzes survival probability based on the number of siblings/spouses aboard.
- **Age Distribution**: Examines the distribution of ages among survivors and non-survivors.
- **Survival Probability by Sex**: Compares survival rates between males and females.
- **Survival Probability by Pclass**: Analyzes survival rates across different ticket classes.
- **Survival Probability by Embarked**: Examines survival rates based on the port of embarkation.

## Data Preprocessing

Data preprocessing steps include:

1. **Handling Missing Values**: 
   - Fill missing values in the `Embarked` column with the most frequent value ('S').
   - Fill missing values in the `Age` column with random values generated from the normal distribution of existing ages.

2. **Encoding Categorical Features**:
   - Convert `Sex` to numerical values (male: 0, female: 1).
   - Convert `Embarked` to numerical values (S: 0, C: 1, Q: 2).

3. **Dropping Unnecessary Columns**: Drop columns that are not needed for modeling.

4. **Splitting Data**: Split the data into training and testing sets.

5. **Feature Scaling**: Standardize the features using `StandardScaler`.

## Modeling

We implement the following classifiers:

- Logistic Regression
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- K-Nearest Neighbors (KNN) Classifier
- Random Forest Classifier

## Results

The accuracy of each classifier is as follows:
Logistic Regression: xx.xx%
- **Logistics Regression :  81.34
-**Support Vector       :  82.09
-**Decision Tree        :  79.1
-**K-NN Classifier      :  80.97
-**Random Forest        :  81.72

## Conclusion

In this project, we explored the Titanic dataset, preprocessed the data, and implemented multiple classifiers to predict survival. We compared the performance of different classifiers and identified the most accurate model.
