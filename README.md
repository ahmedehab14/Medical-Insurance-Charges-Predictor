# Medical Insurance Charges Prediction

## Project Overview
This project aims to analyze a medical insurance dataset to understand the factors influencing insurance charges and to build predictive models for estimating these charges. The dataset is a modified version of the Medical Insurance Price Prediction dataset available on Kaggle.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Objectives](#objectives)
- [Data Cleaning and Processing](#data-cleaning-and-processing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Development](#model-development)
- [Performance Evaluation](#performance-evaluation)
- [Requirements](#requirements)


## Introduction
Medical insurance charges can vary widely based on several factors, including age, gender, body mass index (BMI), number of children, smoking status, and geographical region. This project focuses on cleaning the dataset, performing exploratory data analysis (EDA), and developing predictive models to better understand these relationships.

## Dataset
The dataset contains the following features:
- **Age**: Age of the insured (integer).
- **Gender**: Gender of the insured (mapped to numerical values).
- **BMI**: Body Mass Index of the insured (float).
- **No_of_Children**: Number of children (integer).
- **Smoker**: Smoking status (mapped to numerical values).
- **Region**: Geographical region of the insured (mapped to numerical values).
- **Charges**: Insurance charges in USD (float).

## Objectives
1. Load the data as a pandas DataFrame.
2. Clean the data, addressing missing values and inconsistencies.
3. Perform exploratory data analysis to identify factors affecting insurance charges.
4. Develop single and multi-variable Linear Regression models for prediction.
5. Utilize Ridge Regression to improve model performance.

## Data Cleaning and Processing
- Missing values were handled by replacing them with the mean or mode of respective columns.
- Categorical variables were mapped to numerical values for analysis.
- Data was standardized and prepared for modeling.

## Exploratory Data Analysis
- Conducted visualizations to explore relationships between features and insurance charges.
- Identified key variables that significantly impact the charges.

## Model Development
- Split the dataset into training and testing subsets (80/20).
- Implemented a pipeline using `StandardScaler()`, `PolynomialFeatures()`, and `LinearRegression()`.
- Evaluated models based on \( R^2 \), Mean Absolute Error (MAE), and Mean Squared Error (MSE).

## Performance Evaluation
- **R^2 Score**: 0.8476
- **Mean Absolute Error**: 2963.51
- **Mean Squared Error**: 24872219.07

## Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

