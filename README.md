# Titanic Survival Prediction using Machine Learning

## Overview

This project predicts whether a passenger survived the Titanic disaster using Machine Learning techniques. The model was trained on the Kaggle Titanic dataset and evaluated through the Kaggle competition leaderboard.

## Dataset

Source: Kaggle Titanic - Machine Learning from Disaster

Files used:

* train.csv
* test.csv

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Google Colab

## Data Preprocessing

* Handled missing values in Age, Fare, and Embarked columns
* Removed Cabin due to excessive missing values
* Encoded categorical features using Label Encoding
* Created new features for improved prediction

## Feature Engineering

Created a new feature:

FamilySize = SibSp + Parch + 1

Features used:

* Pclass
* Sex
* Age
* Fare
* Embarked
* SibSp
* Parch
* FamilySize

## Model Used

Random Forest Classifier

### Initial Model

* n_estimators = 100
* Public Score: 0.75358

### Improved Model

* n_estimators = 500
* max_depth = 5
* Added FamilySize feature
* Public Score: 0.78708

## Results

Best Kaggle Public Score: **0.78708 (78.71%)**

The project demonstrates:

* Data cleaning
* Feature engineering
* Classification modeling
* Hyperparameter tuning
* Kaggle competition workflow

## How to Run

1. Clone the repository
2. Install dependencies

pip install pandas numpy scikit-learn matplotlib seaborn

3. Open the notebook
4. Run all cells
5. Generate submission.csv
6. Upload the submission file to Kaggle

## Project Structure

Titanic-ML-Project/
│
├── Titanic.ipynb
├── README.md
├── train.csv
├── test.csv
├── submission_v2.csv

## Future Improvements

* Extract titles from passenger names
* Use cross-validation
* Compare multiple machine learning models
* Implement XGBoost and Gradient Boosting models

## Author

Varun Vaibhav.S

B.Tech CSE (AI & Data Analytics)

Sri Ramachandra Institute of Higher Education and Research
