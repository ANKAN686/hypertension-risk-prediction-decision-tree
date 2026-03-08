# hypertension-risk-prediction-decision-tree
📌 Project Overview

This project builds a Decision Tree classifier to predict whether an individual is at risk of Hypertension (High Blood Pressure) based on health and lifestyle attributes such as age, BMI, salt intake, stress levels, and medical history.

The model uses the Entropy / Information Gain criterion to determine the best splits and classify patients into:

Hypertension Risk → Yes / No

This project demonstrates a complete Machine Learning workflow, including:

Exploratory Data Analysis (EDA)

Data preprocessing

Model training

Model evaluation

Feature importance analysis

📊 Dataset

Dataset: Hypertension Risk Prediction Dataset
Source: Kaggle

The dataset contains health-related information about individuals along with whether they have hypertension.

📋 Input Features
Feature	Description
Age	Patient age in years
Salt_Intake	Daily salt intake (grams)
Stress_Score	Stress level (0–10 scale)
BP_History	Previous blood pressure status
Sleep_Duration	Average hours of sleep per day
BMI	Body Mass Index
Medication	Type of medication taken
Family_History	Family history of hypertension
Exercise_Level	Physical activity level
Smoking_Status	Smoker or Non-smoker
🎯 Target Variable
Variable	Description
Has_Hypertension	Indicates presence of hypertension (Yes/No)
⚙️ Project Workflow
1️⃣ Data Exploration (EDA)

Exploratory Data Analysis was performed to understand the dataset and detect patterns.

Steps Performed

Displayed basic dataset statistics

Checked for missing values

Analyzed feature distributions

📈 Visualizations

Several visualizations were created, including:

Age distribution of patients

BMI vs Hypertension risk

Exercise level vs Hypertension

Salt intake distribution

These plots help identify correlations between lifestyle factors and hypertension risk.

🧹 Data Preprocessing

Several preprocessing steps were applied before training the model.

Handling Missing Values

Missing values were handled using:

Removing incomplete rows

Filling missing values using statistical methods (mean / mode)

Encoding Categorical Variables

Categorical features such as:

BP History

Exercise Level

Smoking Status

Medication

were converted into numerical form using encoding techniques.

Feature Scaling

Numerical variables such as:

Age

BMI

Salt Intake

Stress Score

Sleep Duration

were scaled where necessary.

🌳 Model Building

A Decision Tree Classifier was used to predict hypertension risk.

Splitting Criterion

The model uses Entropy / Information Gain to determine optimal splits.

Training Strategy

Dataset split into Training (80%) and Testing (20%)

Model trained on training data

Evaluated on unseen test data

📉 Model Performance Analysis

To understand model complexity and avoid overfitting, the model was trained with different max_depth values.

Accuracy vs Tree Depth

Training accuracy and validation accuracy were plotted against max_depth.

This helps determine the optimal tree depth.

Observations

Small depth → Underfitting

Large depth → Overfitting

Moderate depth → Best generalization

📊 Evaluation Metrics

The best performing model was evaluated using:

Confusion Matrix

Shows correct and incorrect predictions for:

True Positives

False Positives

True Negatives

False Negatives

Classification Report

Includes the following metrics:

Precision

Recall

F1 Score

Accuracy

These metrics help evaluate how well the model predicts hypertension cases.

🔍 Feature Importance Analysis

Decision Trees provide a measure of feature importance, showing which variables influence predictions the most.

Top 5 Important Features

The most influential features typically include:

Age

BMI

Salt Intake

Stress Score

Family History

Interpretation

These features are medically relevant because:

High salt intake increases blood pressure.

High BMI is associated with obesity-related hypertension.

Family history indicates genetic predisposition.

Stress levels can elevate blood pressure.

Age increases hypertension risk.

📚 Key Learnings

This project helped in understanding:

Exploratory Data Analysis (EDA)

Data preprocessing and encoding

Decision Tree classification

Model evaluation using classification metrics

Feature importance interpretation

Model complexity analysis using max_depth

🚀 Possible Improvements

Future improvements could include:

Using Random Forest or Gradient Boosting

Performing hyperparameter tuning

Applying cross-validation

Improving preprocessing techniques

Adding more health-related features

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Scikit-learn
