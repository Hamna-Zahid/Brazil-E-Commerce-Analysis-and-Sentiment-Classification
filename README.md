# Brazil E-Commerce Analysis and Sentiment Classification

## Overview

This project provides a comprehensive analysis of Brazil's e-commerce landscape using the Olist dataset. The notebook explores customer behavior, geographical trends, payment patterns, and the economic footprint of e-commerce in Brazil. Additionally, it applies **Natural Language Processing (NLP)** techniques to perform sentiment analysis on customer reviews, combining both structured and unstructured data analysis.

## Objectives

- Analyze key metrics such as order volume, payment types, and regional activity.
- Visualize customer and seller distributions across Brazil.
- Preprocess and analyze customer review text data using NLP.
- Build and evaluate sentiment classification models using machine learning.

## Dataset

The analysis is based on the [Olist e-commerce public dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce). The following files are used:

- `olist_customers_dataset.csv`
- `olist_geolocation_dataset.csv`
- `olist_orders_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_products_dataset.csv`
- `olist_sellers_dataset.csv`

## Notebook Structure

### 1. Libraries
Imports all necessary libraries including Pandas, Seaborn, Plotly, Sklearn, LightGBM, and NLP tools.

### 2. Data Reading and Initial Inspection
Loads and previews all datasets. Checks data types, dimensions, and missing values.

### 3. Exploratory Data Analysis (EDA)
- **Order Analysis**: Volume, delivery times, order status.
- **Geographical Distribution**: Map visualizations with `folium`.
- **Economic Insight**: Payment methods and revenue analysis.
- **Word Clouds**: Generated from review comments.

### 4. Natural Language Processing
- Cleaning reviews (regex, stopwords, stemming).
- Feature extraction using CountVectorizer and TF-IDF.
- Labeling and preparing for classification.

### 5. Sentiment Classification
- Train/test split and model training using:
  - Logistic Regression
  - Random Forest
  - LightGBM
  - Naive Bayes
- Evaluation using classification reports and confusion matrices.

### 6. Final Implementation
Wrap-up with pipeline creation, model saving, and results interpretation.

Results
-Identified customer and seller hotspots across Brazil.
-Found strong correlations between payment methods and order value.
-Built effective sentiment analysis models using TF-IDF and LightGBM.
-Achieved classification accuracy >80% for binary sentiment labels.
