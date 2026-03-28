# Titanic Survival Prediction

## 📌 Overview

This project aims to build a machine learning model to predict whether a passenger survived the sinking of the Titanic.

The dataset is split into two groups:

- **Training set (`train.csv`)**
- **Test set (`test.csv`)**

The training set includes the ground truth (`survival`) for each passenger and should be used to train and validate the model.

The test set does **not** include survival outcomes. Your task is to use the trained model to predict survival for each passenger in the test set.

An example submission file (`gender_submission.csv`) is provided, which assumes that all and only female passengers survived.

---

## 📊 Dataset Description

### Target Variable

| Variable   | Definition | Key |
|------------|------------|-----|
| survival   | Survival   | 0 = No, 1 = Yes |

---

### Feature Variables

| Variable  | Definition | Key |
|------------|------------|-----|
| pclass     | Ticket class | 1 = 1st, 2 = 2nd, 3 = 3rd |
| sex        | Sex | |
| age        | Age in years | |
| sibsp      | # of siblings / spouses aboard | |
| parch      | # of parents / children aboard | |
| ticket     | Ticket number | |
| fare       | Passenger fare | |
| cabin      | Cabin number | |
| embarked   | Port of Embarkation | C = Cherbourg, Q = Queenstown, S = Southampton |

---

## 📝 Variable Notes

### pclass
A proxy for socio-economic status (SES):

- **1st** = Upper class  
- **2nd** = Middle class  
- **3rd** = Lower class  

---

### age
- Age is fractional if less than 1.
- If the age is estimated, it is recorded as `xx.5`.

---

### sibsp
Number of siblings or spouses aboard.

Definitions:
- **Sibling** = brother, sister, stepbrother, stepsister
- **Spouse** = husband, wife  
  *(Mistresses and fiancés were ignored)*

---

### parch
Number of parents or children aboard.

Definitions:
- **Parent** = mother, father
- **Child** = daughter, son, stepdaughter, stepson

Note:
- Some children traveled only with a nanny; therefore, `parch = 0` for them.

---

## 🎯 Objective

Using the training data:
- Perform data preprocessing
- Engineer useful features
- Train a machine learning model
- Evaluate model performance

Using the test data:
- Predict survival outcomes
- Generate a submission file with:
  - `PassengerId`
  - `Survived`

---

## 🚀 Suggested Workflow

1. Data exploration (EDA)
2. Handle missing values
3. Feature engineering
4. Model selection (Logistic Regression, Random Forest, XGBoost, etc.)
5. Cross-validation
6. Generate predictions
7. Create submission file

---

## 📁 Expected Submission Format

```csv
PassengerId,Survived
892,0
893,1
894,0
...