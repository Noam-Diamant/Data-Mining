Data Mining Project: Hotel Reservation Cancellations
Overview
This project analyzes hotel reservation data to predict cancellations using various machine learning models. The workflow includes data exploration, cleaning, feature engineering, visualization, and model evaluation. The dataset contains detailed information about hotel bookings, including guest demographics, booking details, and whether the reservation was canceled.
Dataset
Source: hotels_train.csv (training), hotels_test.csv (test)
Rows: ~27,000 (train)
Columns: 18+ features, including:
Reservation details (dates, nights, room type, board type)
Guest details (number of adults/children, repeated guest)
Booking details (lead time, price, purchase type, requests)
Target: is_canceled (0 = not canceled, 1 = canceled)
Data Exploration & Cleaning
Inspected data types, missing values, and attribute distributions
Cleaned and transformed features:
Extracted numeric room type
Encoded categorical variables (board type, purchase type)
Imputed missing values for price and lead_time using statistical and distribution-based methods
Removed outliers and inconsistent dates
Engineered new features (e.g., family size, date split)
Normalized and standardized key features
Visualizations & Insights
Histograms and boxplots for numerical and categorical features
Correlation heatmaps to identify relationships between variables
Target variable (is_canceled) distribution and attribute behavior by cancellation status
Feature importance visualizations for model interpretability
Modeling Approach
Models Used:
Decision Tree (with hyperparameter tuning)
Random Forest (with hyperparameter tuning)
Logistic Regression (with hyperparameter tuning)
Evaluation:
Train/validation split and cross-validation
Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC
Confusion matrices and ROC curves for model comparison
Results (Sample)
Decision Tree accuracy: ~85%
Random Forest accuracy: ~88%
Logistic Regression accuracy: ~80%
Random Forest performed best overall
How to Run
Install dependencies (see below)
Run project.ipynb in Jupyter Notebook or compatible environment
The notebook covers all steps: EDA, cleaning, feature engineering, modeling, and evaluation
Dependencies
Python 3.x
pandas, numpy, matplotlib, seaborn
scikit-learn
Files
project.ipynb: Main analysis and modeling notebook
hotels_train.csv, hotels_test.csv: Data files
DMREPORT.docx, Final project.docx, Transformations.docx: Project reports
TA/TA1-TA7.ipynb: Additional analysis notebooks
Authors
Noam Diamant

