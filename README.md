# credit-risk-prediction-shap
Logistic regression model for credit default prediction with SHAP-based explainability
# 🧠 Credit Risk Prediction with SHAP Explainability

This project uses a logistic regression model to predict whether a credit card customer is likely to **default on payment next month**, based on their financial behavior. To make the predictions transparent and trustworthy, I use **SHAP (SHapley Additive Explanations)** to show how much each feature contributes to each decision.

---

## 🔍 Why I Built This

In finance — especially when it comes to loans and credit — it's not enough for a model to be accurate. You also need to be able to **explain why** it made the decision. This project was built as part of my work to explore **explainable AI** for risk analysis in credit scoring.

---

## 📁 What’s in This Repository

- `credit_risk_model.ipynb` — The full Google Colab notebook:
  - Data preprocessing
  - Model training using logistic regression
  - Evaluation using confusion matrix, F1-score, ROC AUC
  - Explanation with SHAP visualizations (force plot and summary plot)

- `summary_plot.png` — SHAP summary plot showing the most influential features globally.

---

## 📊 Dataset

- Source: [UCI Credit Card Default Dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- Features: credit limit, payment history, bill amounts, demographics
- Target: whether the customer defaulted on their payment (binary classification)

---

## 🧠 What the Model Learned

- **Most predictive feature**: `PAY_0` (repayment status in the previous month)
- High bill amounts and missed payments increase risk
- Higher credit limits and older age reduce risk

Using SHAP, I was able to generate both:
- **Individual explanations** (why this customer was flagged)
- **Global explanations** (which features matter the most overall)

---

## 📦 Tech Stack

- Python (Pandas, Scikit-learn)
- SHAP for explainability
- Google Colab for notebook execution and plotting
- Matplotlib and Seaborn for visuals

---

## ✅ Next Steps

In the future, I’d like to:
- Try more complex models (e.g., XGBoost, LightGBM)
- Apply SMOTE to balance the classes
- Deploy the model using Streamlit or Flask for a front-end demo

---

## 👋 About Me

I'm a Computer Engineering Master's student passionate about the intersection of **AI, explainability, and real-world impact** — especially in fields like finance, risk, and systems security. You can connect with me on [LinkedIn](https://www.linkedin.com/in/joshua-iwu-870054214/).

