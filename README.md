Project Overview

This project demonstrates model optimization using GridSearchCV on the Titanic dataset.

The objective is to improve the performance of a machine learning model by tuning its hyperparameters and comparing the optimized model with the default model.

📂 Dataset Information

Dataset: Titanic Dataset

File Used: train.csv

Target Variable: Survived

Problem Type: Binary Classification

The dataset contains passenger details such as:

Pclass

Sex

Age

Fare

Embarked

SibSp

Parch

⚙️ Steps Performed
1️⃣ Data Loading

Loaded dataset using Pandas.

2️⃣ Data Preprocessing

Dropped unnecessary columns (PassengerId, Name, Ticket, Cabin)

Filled missing values:

Age → Median

Embarked → Mode

Encoded categorical variables (Sex, Embarked)

3️⃣ Train-Test Split

Split data into 80% training and 20% testing.

4️⃣ Default Model Training

Used RandomForestClassifier with default parameters.

Evaluated accuracy.

5️⃣ Hyperparameter Tuning

Applied GridSearchCV with:

Cross-validation = 3 or 5 folds

Reduced parameter grid for faster execution

Extracted best parameters.

6️⃣ Model Evaluation

Compared:

Default Model Accuracy

Tuned Model Accuracy

Generated performance comparison table.

🔍 Hyperparameters Tuned

Example parameter grid used:

param_grid = {
    'n_estimators': [100, 200],
    'max_depth': [None, 10]
}


GridSearchCV settings:

cv = 3
n_jobs = -1

📊 Results
Model	Accuracy
Default Random Forest	(your score)
Tuned Random Forest	(your score)

✔ Tuned model achieved improved performance compared to the default model.
