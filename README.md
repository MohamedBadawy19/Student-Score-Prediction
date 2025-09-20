

📊 Student Score Prediction

This repository contains a machine learning project to analyze and predict student exam performance based on multiple socio-economic, behavioral, and academic factors.

The project leverages Python, pandas, scikit-learn, and visualization libraries to clean the dataset, explore key insights, and build regression models for prediction.


---

📌 Project Overview

Goal: Predict students’ Exam_Score using a variety of input factors such as study hours, attendance, parental involvement, motivation, and socio-economic attributes.

Dataset: Student Performance Factors (6,607 rows, 20 columns).

Approach:

Data cleaning & preprocessing

Exploratory data analysis (EDA)

Feature engineering

Model building (Linear Regression, Ridge Regression, Polynomial Regression)

Model evaluation using error metrics and cross-validation




---

📂 Dataset Description

The dataset includes 20 features that describe student lifestyle, academic factors, and demographics.

Key Features:

Hours_Studied (int) – Number of study hours per week

Attendance (int) – Attendance percentage

Parental_Involvement (categorical: Low/Medium/High)

Access_to_Resources (categorical: Low/Medium/High)

Extracurricular_Activities (Yes/No)

Sleep_Hours (int)

Previous_Scores (int)

Motivation_Level (Low/Medium/High)

Internet_Access (Yes/No)

Tutoring_Sessions (int)

Family_Income (Low/Medium/High)

Teacher_Quality (Low/Medium/High)

School_Type (Public/Private)

Peer_Influence (Positive/Neutral/Negative)

Physical_Activity (int)

Learning_Disabilities (Yes/No)

Parental_Education_Level (High School/College/Postgraduate)

Distance_from_Home (Near/Moderate/Far)

Gender (Male/Female)

Exam_Score (target variable, int)



---

🛠 Project Workflow

1. Data Preprocessing

Removed invalid scores (Exam_Score > 100)

Imputed missing values (Teacher_Quality, Parental_Education_Level, Distance_from_Home) with mode

Encoded categorical variables

Scaled numerical features using MinMaxScaler


2. Exploratory Data Analysis

Distribution plots of exam scores

Correlation heatmaps between numerical variables

Scatter plots (e.g., Hours_Studied vs Exam_Score grouped by gender)

Categorical impact analysis (Parental involvement, income, motivation)


3. Feature Engineering

Polynomial features for non-linear relationships

Normalization and scaling for regression models


4. Modeling

Linear Regression

Ridge Regression (regularized linear model)

Polynomial Regression (with pipeline transformation)

Model validation using K-Fold Cross Validation


5. Evaluation Metrics

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score



---

📈 Results & Insights

Strong positive correlation between Hours Studied, Attendance, Previous Scores and final exam performance.

Socio-economic factors (parental education, family income, resource access) show significant influence.

Polynomial Regression provided better accuracy compared to plain Linear Regression, indicating non-linear relationships.

Regularization (Ridge) helped reduce overfitting and improved model generalization.



---

🚀 Installation & Usage

1. Clone the repository:

git clone https://github.com/your-username/student-score-prediction.git
cd student-score-prediction


2. Install required dependencies:

pip install -r requirements.txt


3. Run the Jupyter Notebook:

jupyter notebook student-score-prediction.ipynb




---

📚 Dependencies

Python 3.11+

pandas

numpy

matplotlib

seaborn

scikit-learn

jupyter



---

📌 Future Improvements

Add classification models for categorical performance levels (e.g., Pass/Fail, Grade prediction)

Hyperparameter tuning with GridSearchCV

Deployment as a web application using Flask/Streamlit

Explainable AI with SHAP/feature importance



---

✨ Acknowledgments

Dataset source: Kaggle – Student Performance Factors

Inspired by educational data mining and predictive analytics research.
