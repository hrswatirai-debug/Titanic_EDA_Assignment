# Titanic Exploratory Data Analysis (EDA) & Survival Prediction

## Project Overview

This project presents a complete **Exploratory Data Analysis (EDA)** of the Titanic Dataset using Python.
The objective is to understand passenger survival patterns, identify influential variables, clean and preprocess the dataset, engineer meaningful features, and build a beginner-friendly predictive model.

The project is designed as a practical introduction to the **real data science workflow**, starting from raw data inspection and ending with basic machine learning.

---

## Objective

The main goals of this assignment are:

* Understand the structure of the Titanic dataset
* Perform systematic exploratory data analysis
* Detect and handle missing values
* Study feature distributions and relationships
* Engineer new useful variables
* Analyze factors influencing survival
* Prepare data for machine learning
* Build a simple predictive model

---

## Problem Statement

The Titanic disaster dataset is a classic **binary classification problem** where the target is to predict whether a passenger survived or not.

### Target Variable

* **Survived**

  * `0` = Did not survive
  * `1` = Survived

---

## Dataset Information

Source: Kaggle Titanic Competition Dataset

The dataset contains passenger-level information such as:

* Passenger Class
* Name
* Sex
* Age
* Fare
* Embarkation Port
* Family Relations
* Survival Status

---

## Tools and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Project Workflow

### 1. Data Loading and Initial Inspection

Performed:

* Dataset import
* Shape analysis
* Column inspection
* Data type identification

Methods used:

```python
df.head()
df.shape
df.info()
df.describe()
```

---

### 2. Data Cleaning and Preprocessing

Handled missing values in:

* Age → Median imputation
* Embarked → Mode imputation
* Cabin → Dropped due to excessive missing values

Removed non-essential columns:

* PassengerId
* Name
* Ticket

Reason:
These columns add limited predictive value in baseline analysis.

---

### 3. Exploratory Data Analysis (EDA)

Studied:

* Passenger age distribution
* Gender distribution
* Passenger class distribution
* Survival distribution

Visualizations used:

* Histograms
* Countplots
* Boxplots
* Barplots
* Heatmaps

---

### 4. Survival Analysis

Survival examined across:

* Gender
* Passenger Class
* Age Groups
* Fare
* Embarkation Port

Key questions explored:

* Did women survive more than men?
* Did higher-class passengers survive more?
* Did children have bet

