#  Learning Log- This document tracks the progress of my Deep Learning journey through a real-world Life Insurance Premium Prediction project.
My goal is to document not just what I built, but also how I learned and improved throughout the project.

## Phase 1 – Dataset Understanding & Preprocessing

### Objective

Prepare the Life Insurance Premium dataset for Deep Learning by cleaning, analyzing, and transforming the data into a model-ready format.

### What I Completed

#### Dataset Exploration

* Loaded the Life Insurance dataset into Pandas.
* Explored data types, missing values, and descriptive statistics.
* Identified numerical columns stored as text and corrected their data types.

#### Exploratory Data Analysis (EDA)

* Visualized numerical feature distributions using histograms.
* Used boxplots to detect outliers.
* Analyzed categorical feature distributions.
* Built a correlation heatmap to understand relationships between features and the target variable.
* Compared insurance premiums for smokers vs. non-smokers to derive business insights.

#### Data Cleaning

* Converted object columns to numerical format.
* Removed extreme outliers from `annual_income` using the IQR method.
* Filled missing numerical values using median imputation.
* Filled missing categorical values using mode imputation.
* Removed non-informative columns (`applicant_id` and `lucky_number`).

#### Feature Engineering & Preprocessing

* Standardized inconsistent values in the `smoker` and `medical_history` columns.
* Applied Label Encoding to categorical features.
* Performed an 80/20 train-test split before scaling to prevent data leakage.
* Standardized numerical features using `StandardScaler`.

### Key Learnings

* Correct data types are essential before performing analysis.
* Median is a better choice than mean for skewed numerical data.
* Outlier removal can improve data quality and model stability.
* Categorical values should be standardized before encoding.
* Train-test split must be done before scaling to avoid data leakage.
* Feature scaling is important for Deep Learning models because features with different ranges can slow or destabilize training.

### Current Status

Dataset cleaned and fully prepared for model training.

### Next Phase

* Build the Deep Learning model.
* Train and evaluate performance.
* Tune hyperparameters.
* Compare results with baseline ML models.
