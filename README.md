# 📊 **Student Score Prediction**

*A comprehensive machine learning project analyzing and predicting student exam performance through socio-economic, behavioral, and academic factors.*

This project leverages **Python**, **pandas**, **scikit-learn**, and advanced visualization libraries to clean datasets, explore insights, and build robust regression models for accurate predictions.

---

## 🎯 **Project Overview**

**Goal:** Predict students' `Exam_Score` using diverse input factors including study hours, attendance, parental involvement, motivation levels, and socio-economic attributes.

**Dataset:** Student Performance Factors *(6,607 rows × 20 columns)*

### **Methodology:**
- 🧹 Data cleaning & preprocessing  
- 🔍 Exploratory data analysis (EDA)  
- ⚙️ Feature engineering  
- 🤖 Model building (Linear, Ridge & Polynomial Regression)  
- 📊 Model evaluation using error metrics and cross-validation  

---

## 📂 **Dataset Overview**

The dataset encompasses **20 comprehensive features** describing student lifestyle, academic performance, and demographic information.

### **🔑 Key Features:**

| **Feature** | **Type** | **Description** |
|-------------|----------|-----------------|
| `Hours_Studied` | *Integer* | Weekly study hours |
| `Attendance` | *Integer* | Attendance percentage |
| `Parental_Involvement` | *Categorical* | Low / Medium / High |
| `Access_to_Resources` | *Categorical* | Low / Medium / High |
| `Extracurricular_Activities` | *Binary* | Yes / No |
| `Sleep_Hours` | *Integer* | Daily sleep duration |
| `Previous_Scores` | *Integer* | Historical academic performance |
| `Motivation_Level` | *Categorical* | Low / Medium / High |
| `Internet_Access` | *Binary* | Yes / No |
| `Tutoring_Sessions` | *Integer* | Number of tutoring sessions |
| `Family_Income` | *Categorical* | Low / Medium / High |
| `Teacher_Quality` | *Categorical* | Low / Medium / High |
| `School_Type` | *Binary* | Public / Private |
| `Peer_Influence` | *Categorical* | Positive / Neutral / Negative |
| `Physical_Activity` | *Integer* | Weekly activity hours |
| `Learning_Disabilities` | *Binary* | Yes / No |
| `Parental_Education_Level` | *Categorical* | High School / College / Postgraduate |
| `Distance_from_Home` | *Categorical* | Near / Moderate / Far |
| `Gender` | *Binary* | Male / Female |
| `Exam_Score` | ***Target*** | **Final exam score** |

---

## 🛠️ **Project Workflow**

### **1. 🧹 Data Preprocessing**
- ❌ Removed invalid scores (`Exam_Score > 100`)
- 🔧 Imputed missing values using **mode** for categorical features
- 🏷️ **Label encoding** for categorical variables
- 📏 **MinMaxScaler** normalization for numerical features

### **2. 🔍 Exploratory Data Analysis**
- 📈 **Distribution analysis** of exam scores
- 🌡️ **Correlation heatmaps** between numerical variables
- 📊 **Scatter plot analysis** (e.g., Hours_Studied vs Exam_Score by gender)
- 🏷️ **Categorical impact assessment** (parental involvement, income, motivation)

### **3. ⚙️ Feature Engineering**
- 🌀 **Polynomial features** for non-linear relationships
- 🎚️ **Normalization and scaling** for regression optimization

### **4. 🤖 Machine Learning Models**
- 📏 **Linear Regression** *(baseline model)*
- 🔒 **Ridge Regression** *(regularized linear model)*
- 🌀 **Polynomial Regression** *(with pipeline transformation)*
- ✅ **K-Fold Cross Validation** for model reliability

### **5. 📊 Evaluation Metrics**
- 📐 **Mean Absolute Error (MAE)**
- 📊 **Mean Squared Error (MSE)**
- 🎯 **Root Mean Squared Error (RMSE)**
- 🎪 **R² Score** *(coefficient of determination)*

---

## 📈 **Key Results & Insights**

### **🔍 Critical Findings:**
- **📚 Strong positive correlation** between `Hours_Studied`, `Attendance`, `Previous_Scores` and final performance
- **🏠 Socio-economic factors** (parental education, family income, resource access) demonstrate significant influence
- **🌀 Polynomial Regression** outperformed Linear Regression, revealing important non-linear relationships
- **🔒 Ridge Regularization** effectively reduced overfitting and enhanced model generalization

---

## 🚀 **Installation & Usage**

### **1. Clone Repository**
```bash
git clone https://github.com/your-username/student-score-prediction.git
cd student-score-prediction
```

### **2. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3. Launch Analysis**
```bash
jupyter notebook student-score-prediction.ipynb
```

---

## 📚 **Dependencies**

```
Python 3.11+
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

## 🔮 **Future Enhancements**

- 🎯 **Classification models** for performance categories *(Pass/Fail, Grade levels)*
- 🎛️ **Hyperparameter optimization** with GridSearchCV
- 🌐 **Web deployment** using Flask/Streamlit
- 🔍 **Explainable AI** integration with SHAP/feature importance analysis
- 📱 **Interactive dashboards** for real-time predictions

---

## ✨ **Acknowledgments**

**Dataset Source:** [Kaggle – Student Performance Factors](https://kaggle.com)  
**Inspiration:** Educational data mining and predictive analytics research

---
