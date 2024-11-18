# Project: Lead Conversion Analysis & Restaurant Demand Analysis

## Overview

This repository contains two projects focused on data analysis and machine learning to address business challenges in the EdTech and Food Delivery industries.

---

### 1. Lead Conversion Analysis for ExtraaLearn

#### Context
The EdTech industry is growing rapidly, with the online education market expected to reach $286.62 billion by 2023. ExtraaLearn, a startup offering programs in cutting-edge technologies, aims to identify which leads are most likely to convert to paid customers to optimize resource allocation and improve lead nurturing strategies.

#### Objective
- Analyze the leads data to identify conversion likelihood.
- Build a machine learning model to predict lead conversions.
- Identify factors driving conversions.
- Develop a profile for leads likely to convert.

#### Data Description
The dataset includes attributes such as:
- **Demographics**: Age, current occupation.
- **Interaction Details**: First interaction channel, profile completion percentage, website visits, time spent on the website, last activity.
- **Marketing Influence**: Exposure to print and digital media, educational channels, referrals.
- **Target Variable**: Lead conversion status (1 = Converted, 0 = Not converted).

### 2. Restaurant Demand Analysis for FoodHub

#### Context
The increasing number of restaurants and online food delivery demand in New York has created opportunities for food aggregator companies like FoodHub. By analyzing customer order data, FoodHub seeks to enhance customer experience and restaurant demand prediction.

#### Objective
- Analyze the order data to identify key patterns and trends.
- Address business questions to improve customer experience and restaurant demand forecasting.

#### Data Description
The dataset includes:
- **Order Details**: Unique order ID, customer ID, restaurant name, cuisine type, cost.
- **Timing**: Day of the week (weekday/weekend), food preparation time, delivery time.
- **Customer Feedback**: Ratings out of 5.

 Order Data Analysis: Key Patterns and Trends

## Objective
The goal of this project is to analyze the order data from the restaurant to identify key patterns and trends, which will help in answering business questions related to improving customer experience and restaurant demand forecasting.

### Key Business Questions:
1. How can customer experience be improved?
2. How can restaurants forecast demand better?

## Approach

### 1. Data Collection & Preparation
- **Order Data**: Data is collected from restaurant orders, including:
  - Order timestamp
  - Customer details (e.g., demographics, order frequency)
  - Meal types and order sizes
  - Delivery times and statuses (e.g., canceled, delivered)
  
- **Data Preprocessing**:
  - Handle missing values and outliers
  - Standardize time zones and order details
  - Preprocess text if necessary (e.g., reviews or feedback)

### 2. Exploratory Data Analysis (EDA)
We conducted an in-depth exploration of the order data to uncover patterns and trends:

- **Key Patterns**:
  - Popular meal types and ingredients
  - Peak order hours/days of the week
  - Delivery times and customer satisfaction levels
  
- **Trends**:
  - Seasonal demand fluctuations (e.g., holidays, special events)
  - Correlation between promotions/discounts and order frequency

### 3. Feature Engineering
We created new features based on domain knowledge:
- **Day of the week**: Weekday vs. weekend orders
- **Order size**: Small/Medium/Large categories
- **Customer proximity**: Distance from restaurant
- **Discount/Promotions**: Impact of promotions on order frequency

### 4. Model Development
We used machine learning models to classify order data and make predictions:

- **Random Classifier**:
  - Used as a baseline model to evaluate the effectiveness of the classification tasks.
  - Randomly assigns labels to simulate predictions, which we compare against more refined models.

- **Decision Trees/Random Forest**:
  - Aimed to predict significant outcomes such as:
    - Predicting order cancellations
    - Identifying high-demand time periods
    - Forecasting order sizes
  
- **Pruning**:
  - Applied pruning techniques to decision tree models to remove branches that do not contribute significantly to prediction accuracy, thus reducing model complexity and overfitting.

### 5. Results & Insights
- Identified peak order times and days.
- Found correlations between promotional offers and increased order volume.
- Gained insights into the impact of delivery times on customer satisfaction.

### 6. Business Implications
- **Improving Customer Experience**: 
  - Recommendations for adjusting restaurant working hours based on peak demand times.
  - Tailoring promotions to customer preferences and ordering behavior.
  
- **Demand Forecasting**:
  - Use predictive models to adjust staffing levels and inventory management during high-demand periods.
  - Plan for seasonal fluctuations and unexpected surges in demand.

## Installation and Setup

### Requirements:
- Python 3.x
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, etc.


