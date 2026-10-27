# Student Mental Health Score Predictor 🧠📊

An end-to-end Machine Learning project designed to analyze student habits, social media usage patterns, and predict their mental health impact scores.

---

## 📌 Project Overview
With the increasing integration of digital platforms into students' daily routines, understanding the relationship between online behavior and psychological well-being is critical. This project processes behavioral data, evaluates multiple regression models, and exports an end-to-end inference pipeline for predictions.

---

## 🛠️ Tech Stack & Libraries
- **Language:** Python
- **Environment:** Jupyter Notebook / Visual Studio Code
- **Data Analysis & Preprocessing:** Pandas, NumPy, Scikit-learn
- **Machine Learning Algorithms:** 
  - Linear Regression
  - Random Forest Regressor (Tuned via RandomizedSearchCV)
- **Model Serialization:** Joblib

---

## 📈 Model Performance & Evaluation

The models were evaluated using $R^2$ Score, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE):

| Model | Testing $R^2$ | Training $R^2$ | MAE | RMSE |
| :--- | :---: | :---: | :---: | :---: |
| **Linear Regression** | 0.7398 | 0.7237 | 0.5362 | 0.6760 |
| **Random Forest (Default)** | 0.8776 | 0.9808 | 0.3472 | 0.4637 |
| **Random Forest (Tuned)** | 0.8650 | 0.9547 | 0.3689 | 0.4869 |

> The tuned Random Forest model provides a robust balance, minimizing overfitting while maintaining high predictive accuracy on unseen test data.

---

## 📁 Repository Structure
Serialized trained model & pipeline
├── ML_Project.ipynb                            # End-to-end data analysis & modeling notebook
├── Student Social Media And Mental Health...csv # Dataset
└── README.md                                   # Project documentation

---

## 🚀 How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/nibadita705/ML_MODEL-BUILD-Project.git](https://github.com/nibadita705/ML_MODEL-BUILD-Project.git)
   cd ML_MODEL-BUILD-Project
2. **Install required dependencies:**
   pip install numpy pandas scikit-learn joblib
3. **Load the saved model in Python:**
   import joblib

# Load pipeline
model = joblib.load('Mental_Health_Model.pkl')

# Predict on new student data
# predictions = model.predict(new_data)
 
