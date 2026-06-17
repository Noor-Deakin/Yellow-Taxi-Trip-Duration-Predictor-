# Yellow-Taxi-Trip-Duration-Predictor-
End-to-end data wrangling and predictive modelling pipeline built on 11M+ NYC Yellow Taxi trip records (Jan–Mar 2026). Covers data cleaning, feature engineering, and trip duration prediction using Linear Regression and Random Forest. Achieved R² = 0.79 with Random Forest. Built as part of SIT220 Data Wrangling at Deakin University.

Overview
Predicts taxi trip duration in minutes using trip attributes available at pickup time. Trip duration was engineered from raw timestamps as it doesn't exist in the dataset directly.

Dataset
Source: NYC TLC Trip Record Data — Yellow Taxi, Jan–Mar 2026
Raw size: 11,077,206 rows | Cleaned size: 7,572,801 rows

What the Pipeline Does
Cleaned corrupt records: bad timestamps, negative fares, zero passengers, invalid distances
Engineered target variable (trip_duration) and temporal features (hour, day of week, rush hour, weekend)
Caught and removed a data leakage issue (trip speed derived from target variable)
Trained Linear Regression (baseline) vs Random Forest on a 300K sample

Tech Stack
Python, Pandas, Scikit-learn, Matplotlib, Seaborn, Jupyter

Author
Gurnoor Singh — Deakin University, Bachelor of Computer Science
