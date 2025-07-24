**Tobacco & Mortality Prediction – README**

**What This Project Is About**:

This project looks at the relationship between tobacco use and mortality over time. We used data from multiple sources and applied machine learning to predict whether mortality rates would be high or low based on tobacco-related factors. It’s a step toward understanding how smoking habits, prescriptions, and affordability affect health outcomes.

**Project Goal**:

To predict high or low mortality using tobacco-related data, and uncover which factors — like price index, prescriptions, or age groups — contribute most to those outcomes.

**What the Notebook Does**:

Loads and cleans data from multiple CSV files (admissions, fatalities, smokers, prescriptions, etc.)

Merges them into one structured dataset

Handles missing values, outliers, and scales numeric data

Creates a High_Mortality label for classification

Builds a Random Forest model to predict mortality risk

Tunes the model using GridSearchCV

Explains results with SHAP values to show which features mattered most

Saves the final model as rf_mortality_model.pkl

**Key Insights**:

Features like tobacco affordability and prescription patterns play a big role in mortality outcomes

The model performed well in classifying high vs. low mortality

SHAP helped explain the model’s decisions in a visual, transparent way

**Tools & Libraries Used**:

Pandas, NumPy – data wrangling

Matplotlib, Seaborn – data visualization

Scikit-learn – machine learning pipeline

SHAP – explainable AI

Joblib – saving the model

**Required Files**:

Make sure the following CSV files are present before running the notebook:

admissions.csv

fatalities.csv

metrics.csv

prescriptions.csv

smokers.csv

**How to Use It**:

Open the notebook tobacco_mortality_prediction (1).ipynb in Jupyter or Colab

Upload the required CSV files

Run the notebook step-by-step

The trained model (rf_mortality_model.pkl) will be saved at the end
