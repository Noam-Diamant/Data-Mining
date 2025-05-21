# Data Mining Project: Hotel Reservation Cancellations

## Overview
This project analyzes hotel reservation data to predict cancellations using various machine learning models. The workflow includes data exploration, cleaning, feature engineering, visualization, and model evaluation. The dataset contains detailed information about hotel bookings, including guest demographics, booking details, and whether the reservation was canceled.\n\n## Dataset
- **Source:** `hotels_train.csv` (training), `hotels_test.csv` (test)
- **Rows:** ~27,000 (train)
- **Columns:** 18+ features, including:
    - Reservation details (dates, nights, room type, board type)
    -  Guest details (number of adults/children, repeated guest)
    - Booking details (lead time, price, purchase type, requests)
    - Target: `is_canceled` (0 = not canceled, 1 = canceled)\n\n## Data Exploration & Cleaning
    - Inspected data types, missing values, and attribute distributions
    -  Cleaned and transformed features:
    - Extracted numeric room type
    - Encoded categorical variables (board type, purchase type)
    - Imputed missing values for `price` and `lead_time` using statistical and distribution-based methods
    - Removed outliers and inconsistent dates
    - Engineered new features (e.g., family size, date split)
    - Normalized and standardized key features
## Visualizations & Insights
- Histograms and boxplots for numerical and categorical features
- Correlation heatmaps to identify relationships between variables
- Target variable (`is_canceled`) distribution and attribute behavior by cancellation status
- Feature importance visualizations for model interpretability
## Modeling Approach
**Models Used:**
- Decision Tree (with hyperparameter tuning)
- Random Forest (with hyperparameter tuning)
- Logistic Regression (with hyperparameter tuning)\
**Evaluation:**
  - Train/validation split and cross-validation\n  - Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC\n  - Confusion matrices and ROC curves for model comparison\n\n## Results (Sample)\n- Decision Tree accuracy: ~85%\n- Random Forest accuracy: ~88%\n- Logistic Regression accuracy: ~80%\n- Random Forest performed best overall\n\n## How to Run\n1. Install dependencies (see below)\n2. Run `project.ipynb` in Jupyter Notebook or compatible environment\n3. The notebook covers all steps: EDA, cleaning, feature engineering, modeling, and evaluation\n\n## Dependencies\n- Python 3.x\n- pandas, numpy, matplotlib, seaborn\n- scikit-learn\n\n## Files\n- `project.ipynb`: Main analysis and modeling notebook\n- `hotels_train.csv`, `hotels_test.csv`: Data files\n- `DMREPORT.docx`, `Final project.docx`, `Transformations.docx`: Project reports\n- `TA/TA1-TA7.ipynb`: Additional analysis notebooks\n\n## Authors\n- Noam Diamant\n\n---\nThis project demonstrates a full data mining pipeline for a real-world business problem, from raw data to actionable insights and predictive modeling.\n
