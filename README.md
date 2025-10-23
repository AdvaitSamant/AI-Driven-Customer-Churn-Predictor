# 💼 AI-Driven Customer Churn Predictor & Retention Dashboard

## Overview
This project is a full-stack **AI-powered churn prediction and retention tool** designed to help businesses identify customers at risk of leaving and generate personalized retention strategies. It combines **machine learning, explainable AI, and an interactive dashboard** to deliver actionable business insights.

---

## Features
- **Predictive Modeling:**  
  - Uses a **Random Forest classifier** trained on customer demographics, account info, product usage, satisfaction scores, complaints, credit info, and more to predict churn probability.  
- **Explainable AI:**  
  - **SHAP (SHapley Additive exPlanations)** shows feature contributions, helping analysts understand *why* a customer might churn.  
- **AI-Powered Retention Strategy:**  
  - Integrates **OpenAI GPT-3** to generate personalized retention suggestions for high-risk customers.  
- **Interactive Dashboard:**  
  - Built with **Dash & Plotly**.  
  - Features CSV upload, row-level churn predictions, SHAP feature importance charts, and AI-driven retention strategies.  
- **Professional Look & Feel:**  
  - Desktop-style usability with Bootstrap styling for a clean, professional BI tool experience.

---

## Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn (Random Forest)  
- SHAP (Explainable AI)  
- Dash & Plotly (Interactive Dashboard)  
- OpenAI API (Retention Strategy Generation)  
- Bootstrap (Styling)

---

## Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/your-username/churn-predictor.git
cd churn-predictor
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Train the Model
```bash
python train_model.py
```

### 4. Run Dashboard
```bash
python app_dash.py
```

### 5. Upload Your Dataset

Upload your customer CSV in the dashboard

Select a row to predict churn

View churn probability, SHAP feature importance, and AI retention strategy

Dataset
The app expects a CSV file with the following columns:
```bash
RowNumber, CustomerId, Surname, CreditScore, Geography, Gender, Age, Tenure, Balance, 
NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary, Exited, Complain, 
Satisfaction Score, Card Type, Point Earned
```
Exited: Target column (1=churned, 0=active)

### How It Works: 

1. ML Model: Random Forest predicts customer churn.

2. Feature Scaling & Encoding: Categorical features are label encoded and numerical features scaled.

3. SHAP Explainability: Visualizes feature contributions per customer prediction.

4. AI Retention: GPT-3 generates personalized strategies for high-risk customers.

5. Dash Dashboard: Interactive, professional interface for analysts and decision-makers.

Why It Stands Out: 

1. Combines predictive modeling + explainable AI + AI-generated business recommendations.

2. Professional, interactive dashboard for real-time decision-making.

3. End-to-end workflow for business analysts + AI integration.

License
This project is licensed under the MIT License
