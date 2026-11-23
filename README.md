# Medical Appointment No-Show Analysis

A data analysis and machine learning project investigating factors influencing patient attendance at scheduled medical appointments and predicting appointment no-shows.

## Project Overview

The project uses a dataset containing **106,987 medical appointments** and 15 variables, including demographic information, medical conditions, appointment scheduling details, and SMS reminders.

The main objectives are:
- Explore the dataset and identify patterns affecting appointment attendance.
- Investigate relationships between patient characteristics and no-show rates.
- Perform statistical hypothesis testing.
- Build and evaluate classification and regression models.

## Methods & Technologies

**Python** · Pandas · NumPy · SciPy · Matplotlib · Plotly · Scikit-learn · Statsmodels

The analysis includes:
- Exploratory Data Analysis (EDA) and interactive visualizations.
- Statistical hypothesis testing (Welch's t-test, Chi-square test, Mann–Whitney U test).
- Feature engineering and data preprocessing.
- Machine learning models:
  - Gaussian Naive Bayes
  - Random Forest
  - Histogram Gradient Boosting
  - Multiple Linear Regression
  - Poisson Regression

## Key Findings

- Appointment waiting time is the strongest predictor of patient attendance.
- Older patients generally have higher attendance rates.
- Gender and chronic medical conditions show relatively weak associations with attendance.
- SMS reminders are associated with higher no-show rates, largely due to confounding with appointment waiting time.
- Classification models achieve approximately **80% accuracy**, but struggle to identify actual no-shows due to class imbalance.

## Repository Structure

- `main_appointments.ipynb` – Complete analysis, visualizations, statistical tests, and model evaluation.
- `healthcare_noshows_appointments.csv` – Source dataset required to run the notebook.

## Running the Project

Install the required dependencies:

```bash
pip install pandas numpy scipy matplotlib plotly scikit-learn statsmodels jupyter
```

Place the dataset in the same directory as the notebook, then launch Jupyter:

```bash
jupyter notebook main_appointments.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.