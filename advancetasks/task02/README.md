# Customer Churn Prediction using Machine Learning

## Overview

This project builds a **Customer Churn Prediction System** using **Logistic Regression** to predict whether a telecom customer is likely to leave the service.

The model is trained on the **Telco Customer Churn Dataset** and deployed with an interactive **Gradio Web App**.

---

## Dataset

**Dataset Source:** OpenML – Telco Customer Churn Dataset

### Target Variable

* **Churn**

  * Yes → Customer likely to leave
  * No → Customer likely to stay

---

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Joblib
* Gradio

---

## Machine Learning Pipeline

The project uses a complete preprocessing + training pipeline:

1. Data Cleaning
2. Train-Test Split
3. Feature Scaling for Numerical Columns
4. One-Hot Encoding for Categorical Columns
5. Logistic Regression Classification

---

## Model Performance

### Accuracy

82.4%

### Classification Metrics

* Precision, Recall, and F1-Score calculated for churn prediction

---

## Features Used

* Gender
* Senior Citizen Status
* Partner / Dependents
* Tenure
* Phone Service
* Internet Service
* Online Security / Backup
* Device Protection
* Tech Support
* Streaming Services
* Contract Type
* Paperless Billing
* Payment Method
* Monthly Charges
* Total Charges

---

## Model Saving

The trained pipeline is saved using:

```bash id="2rj8fa"
churn_pipeline.pkl
```

---

## Gradio Web App

Interactive interface allows users to:

* Input customer details
* Get instant churn prediction
* Test multiple customer profiles

---

## How to Run

### Install Dependencies

```bash id="8vsekn"
pip install scikit-learn pandas joblib gradio
```

### Run Project

```bash id="x7t6k3"
python churn_prediction.py
```

---

## Sample Output

Input Customer Data → Prediction:

```bash id="2jl0o6"
Churn Prediction: Yes
```

---

## Project Workflow

1. Load Telco Customer Churn Dataset
2. Preprocess Data
3. Train Logistic Regression Model
4. Evaluate Model
5. Save Trained Pipeline
6. Launch Gradio Prediction App

---

## Future Improvements

* Try advanced models (Random Forest, XGBoost)
* Improve feature engineering
* Deploy on Hugging Face / Streamlit Cloud
* Add probability/confidence score to predictions

---

## Author

Arfa Imran
