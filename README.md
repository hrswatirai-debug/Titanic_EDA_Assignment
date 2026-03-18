# Titanic Exploratory Data Analysis (EDA) & Survival Prediction

## Project Overview

This project presents a complete **Exploratory Data Analysis (EDA)** of the Titanic Dataset using Python.
The objective is to understand passenger survival patterns, identify influential variables, clean and preprocess the dataset and engineer meaningful features.

The project is designed as a practical introduction to the **real data science workflow**.

---

## Objective

The main goals of this assignment are:

* Understand the structure of the Titanic dataset
* Perform systematic exploratory data analysis
* Detect and handle missing values
* Study feature distributions and relationships
* Engineer new useful variables
* Analyze factors influencing survival


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
* Did children have better survival chances?

---

### 5. Feature Engineering

Created new features:

### FamilySize

```python
FamilySize = SibSp + Parch + 1
```

Purpose:
To capture travel-group influence on survival.

Additional analysis performed:

* Survival vs Family Size
* Family Size correlation with survival

---

### 6. Correlation Analysis

Generated correlation matrix to understand relationships among numeric variables.

Visualization:

```python
sns.heatmap()
```

Used to identify variables with strongest relationship to survival.

---

## Key Insights

### Survival Patterns Observed

* Female passengers had significantly higher survival rates
* First-class passengers survived more often than third-class passengers
* Children showed relatively better survival probability
* Passengers traveling in small families often survived more than those alone or in very large groups

---

## Learning Outcomes

This project demonstrates practical understanding of:

* Data cleaning logic
* Missing value strategies
* Feature engineering basics
* Visualization interpretation
* Statistical reasoning

---

## Repository Structure

```text
Titanic-EDA/
│── Titanic_EDA.ipynb
│── train.csv
│── README.md
```

---

## Future Improvements

Possible next enhancements:

* Title extraction from passenger names
* Cabin deck extraction
* Advanced feature engineering
* Random Forest model
* Cross-validation
* Hyperparameter tuning

---

## Why This Project Matters?

The Titanic dataset remains one of the most effective beginner datasets because it teaches how multiple factors interact in real-world prediction:

* social class
* demographics
* missing data
* feature relationships

It is an ideal foundation for developing practical data science thinking.

---

## Author

**Swati Rai**

---

## Keywords

Python EDA Titanic Dataset Machine Learning Data Cleaning Feature Engineering Survival Analysis Pandas Seaborn

Python EDA Titanic Dataset Machine Learning Data Cleaning Feature Engineering Survival Analysis Pandas Seaborn
`Python` `EDA` `Titanic Dataset` `Machine Learning` `Data Cleaning` `Feature Engineering` `Survival Analysis` `Pandas` `Seaborn` `Scikit-learn`
