# Logistic Regression Model for Predicting 10-Year Risk of Coronary Heart Disease (CHD)

## Overview
This project implements a **Logistic Regression model** to predict the **10-year risk of Coronary Heart Disease (CHD)**. The model is trained on a dataset consisting of **4,328 records**, where the target variable is binary:
- **1**: High risk of CHD (Yes)
- **0**: Low risk of CHD (No)

## Dataset
The dataset contains various health and demographic features that contribute to CHD risk. Some of the key features may include:
- Sex: male or female(Nominal)
- Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)
Behavioral
- Current Smoker: whether or not the patient is a current smoker (Nominal)
- Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.)
Medical( history)
- BP Meds: whether or not the patient was on blood pressure medication (Nominal)
- Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)
- Prevalent Hyp: whether or not the patient was hypertensive (Nominal)
- Diabetes: whether or not the patient had diabetes (Nominal)
Medical(current)
- Tot Chol: total cholesterol level (Continuous)
- Sys BP: systolic blood pressure (Continuous)
- Dia BP: diastolic blood pressure (Continuous)
- BMI: Body Mass Index (Continuous)
- Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.)
- Glucose: glucose level (Continuous)
Predict variable (desired target)
- 10 year risk of coronary heart disease CHD (binary: “1”, means “Yes”, “0” means “No”)

## Model Performance
The Logistic Regression model achieves an **accuracy of 84%**, indicating a strong predictive capability. However, given the class distribution, accuracy alone may not be sufficient. 

### Hyperparameter Tuning
To further improve the model's accuracy, **Grid Search CV** was used for hyperparameter tuning. This optimization improved the accuracy score to **85%** from the initial **84%**.


## Steps for training a model
1. **Load the dataset**
2. **Preprocess the data** (handle missing values, encode categorical variables, scale features if necessary)
3. **Train the Logistic Regression model**
4. **Evaluate the model** using accuracy, recall, precision, and ROC-AUC
5. **Perform Hyperparameter Tuning** using GridSearchCV


## Conclusion
This logistic regression model provides a baseline approach to predicting CHD risk with **85% accuracy** after hyperparameter tuning. 


