# Heart Disease Prediction using Machine Learning

# Project Overview

Heart disease is one of the leading causes of death worldwide. Early detection of heart disease can significantly improve treatment outcomes and reduce mortality rates.

The objective of this project is to build machine learning models that can predict whether a patient is likely to have heart disease based on various medical attributes.

Multiple machine learning algorithms were implemented and compared to determine which model performs best for heart disease prediction.

# Dataset Description

The dataset contains medical attributes of patients that are commonly used in cardiovascular diagnosis.

## Project Workflow

The project followed a structured machine learning pipeline:

1️⃣ Import Libraries and Load Dataset

In the first step, essential Python libraries for data analysis, visualization, and machine learning are imported. The heart disease dataset is then loaded using Pandas for further analysis.

The dataset contains patient health attributes such as age, cholesterol level, blood pressure, chest pain type, and maximum heart rate, which are used as input features for prediction.

The target variable indicates whether the patient has heart disease:

1 → Presence of heart disease

0 → No heart disease

2️⃣ Data Preprocessing

Before training the models, the dataset was cleaned and prepared for machine learning.

The preprocessing stage included:

Removing unnecessary columns if present

Separating features (X) and target variable (y)

Checking for missing values

Ensuring all variables are in a suitable format for model training

Proper preprocessing helps improve model performance and ensures the data is ready for training.

3️⃣ Train-Test Split

To evaluate model performance properly, the dataset was divided into training and testing sets.

Training Data → Used to train the machine learning models

Testing Data → Used to evaluate how well the model performs on unseen data

The split helps prevent overfitting and ensures the model can generalize to new data.

Typically:

80% Training Data

20% Testing Data

4️⃣ Feature Scaling

Feature scaling was applied to normalize the input variables so that all features contribute equally to the model.

This is particularly important for algorithms like Logistic Regression

StandardScaler was used to transform the data so that features have:

Mean = 0

Standard Deviation = 1

Scaling helps improve model stability and convergence during training.

5️⃣ Model Training and Evaluation

In the final stage, multiple machine learning models were trained using the processed dataset.

The models implemented include:

Logistic Regression

Random Forest

XGBoost

Each model was evaluated using the following performance metrics:

Accuracy – Overall correctness of the model

Precision – Percentage of predicted positive cases that were correct

Recall – Ability of the model to detect actual positive cases

F1 Score – Balance between precision and recall

These metrics provide a comprehensive evaluation of the models, especially for healthcare prediction tasks.

The results were also visualized using a bar chart comparison, making it easier to compare model performance.

## Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 0.852    | 0.871     | 0.844  | 0.857    |
| Random Forest       | 0.836    | 0.844     | 0.844  | 0.844    |
| XGBoost             | 0.820    | 0.862     | 0.781  | 0.820    |


 Insights:
 # Logistic Regression performed the best overall, achieving the highest accuracy and F1-score.
 # Random Forest provided balanced performance across all evaluation metrics.
 # XGBoost achieved high precision, indicating fewer false positive predictions, but slightly lower recall.

These results demonstrate how different algorithms behave when applied to medical prediction problems.
 # Visualization:
A bar chart was created to visually compare the performance of all models across evaluation metrics (Accuracy, Precision, Recall, and F1 Score). This visualization helps clearly understand which model performs best.
# Technologies Used:
* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

# Conclusion

This project demonstrates how machine learning techniques can be applied to healthcare datasets to assist in early detection of heart disease. By comparing multiple models and analyzing performance metrics, the study highlights how predictive models can support medical decision-making.

