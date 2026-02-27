# 🏥 Health Insurance Payment Prediction App

An end-to-end Machine Learning web application that predicts estimated health insurance payment amounts based on user demographic and medical details.

This project demonstrates the complete ML lifecycle — from data preprocessing and model training to hyperparameter tuning and deployment using Streamlit.

---

## 🚀 Live Application

(You can add deployment link here later)

---

## 📌 Project Overview

This application uses supervised regression models to estimate insurance claim/payment amounts based on:

- Age
- Gender
- BMI
- Blood Pressure
- Diabetic Status
- Number of Children
- Smoking Status

Multiple models were trained and compared, and the best-performing model was deployed through an interactive Streamlit interface.

---

## 🧠 Machine Learning Workflow

### 1️⃣ Data Preprocessing

- Label Encoding for categorical variables
- Standard Scaling for numerical features
- Train-Test split
- Feature engineering using PolynomialFeatures

### 2️⃣ Models Trained

- Linear Regression
- Polynomial Regression
- Random Forest Regressor
- Support Vector Regressor (SVR)
- XGBoost Regressor

### 3️⃣ Model Selection

- Hyperparameter tuning using `GridSearchCV`
- Cross-validation (CV = 3)
- Evaluation using R² score
- Best model selected based on performance

---

## 📊 Model Performance

| Model                 | R² Score |
| --------------------- | -------- |
| Linear Regression     | ~0.75    |
| Polynomial Regression | ~0.80    |
| Random Forest         | ~0.83    |
| XGBoost               | ~0.85    |

(XGBoost performed best on the test set.)

---

## 🖥️ Deployment

The application is deployed using **Streamlit**, providing:

- Interactive form-based input
- Real-time prediction
- Clean UI layout
- Integrated preprocessing pipeline

All preprocessing objects (scaler, encoders) and the trained model are saved using `joblib` to ensure consistency between training and deployment.

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Streamlit
- Joblib

---

## 📂 Project Structure

health-insurance-app/
│
├── app.py
├── best_model.pkl
├── scaler.pkl
├── label_encoder_gender.pkl
├── label_encoder_diabetic.pkl
├── label_encoder_smoker.pkl
├── notebook.ipynb
├── requirements.txt
└── README.md

---

## ▶️ How to Run Locally

### 1️⃣ Clone the repository

git clone https://github.com/tainytomcruise/health-insurance-app.git
cd health-insurance-app

### 2️⃣ Create virtual environment

python -m venv ml_env
source ml_env/bin/activate

### 3️⃣ Install dependencies

pip install -r requirements.txt

### 4️⃣ Run the app

streamlit run app.py

---

## 📈 Key Learnings

- End-to-end ML pipeline building
- Handling categorical encoding during deployment
- Hyperparameter tuning with GridSearchCV
- Model comparison and evaluation
- Converting ML model into production-ready web app
- Debugging environment and dependency conflicts

---

## 🔮 Future Improvements

- Add model explainability (SHAP)
- Deploy on Streamlit Cloud / Render
- Add input validation & better UI design
- Implement logging and monitoring
- Add REST API endpoint using FastAPI

---

## 👤 Author

**Mayank Sahu**  
GitHub: https://github.com/tainytomcruise

---

⭐ If you found this project useful, consider giving it a star!
