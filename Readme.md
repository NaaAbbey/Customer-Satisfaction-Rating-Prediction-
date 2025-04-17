# 📊 Customer Satisfaction Prediction 

This project uses machine learning models to predict customer satisfaction ratings (1 to 5, with 0 for unresolved cases) based on support ticket data. It explores classification approaches and ordinal regression techniques to handle the ordinal nature of the ratings.

---

## 📁 Dataset

- **Source**: Unified Mentor Google Drive
- **Features**: Ticket category, time to respond, ticket description, product purchased, first response time, ticket priority, etc.
- **Target**: Customer Satisfaction Rating (0 to 5, where 0 = unresolved)

---

## 🎯 Objective

To predict customer satisfaction scores based on features derived from support tickets, aiding support teams in improving service quality and early identification of dissatisfaction trends.

---

## 🔍 Techniques Used

- Preprocessing:
  - Imputation for missing values
  - Encoding categorical variables
  - Feature scaling where needed
- Feature engineering
- Multi-class classification
- Ordinal Regression
- Evaluation using accuracy, MAE, confusion matrix, and visualizations

---

##  Models Used
- Logistic Regression        
- Random Forest Classifier  
- XGBoost Classifier
- LightGBM Classifier        
- Ordinal Regression        

---

## 📈 Model Performance Summary

- **Best Accuracy**: ~21% (vs. baseline 18%)
- **Best MAE**: ~1.15 (lower is better)
- **Ordinal regression** performed best against resolved tickets; however, predicted mostly central classes (rating 3)
- **Inclusion of unresolved cases** as class 0 improved model learning

---

## 📊 Tableau Dashboard

Includes:
- Rating distribution across different categories
- Average satisfaction per category
- Breakdown of predicted vs. actual satisfaction
- Escalation vs. satisfaction impact

> Dashboard Link: _([Tableau Dashboard](https://public.tableau.com/app/profile/daisy.abbey/viz/CustomerSatisfactionPredictionDashboard/CustomerSatisfactionPredictionDashboard?publish=yes))_

---

## 📌 Key Takeaways

- Satisfaction prediction is feasible, though challenging due to class imbalance and subjectivity.
- Ordinal models are better suited for ordered targets.
- Including unresolved tickets helped the models generalize better.
- Feature importance from tree models offers actionable insights for support strategy.

---

## 💾 How to Run

1. Clone the repo:
    ```bash
    git clone https://github.com/NaaAbbey/customer-satisfaction-prediction.git
    cd customer-satisfaction-prediction
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Open and run the notebook:
    ```
    jupyter notebook Notebook.ipynb
    ```

---

## ✉ Contact 
For feedback or collaboration: [Daisy Abbey] | _([LinkedIn](https://www.linkedin.com/in/daisy-a-6394a1282))_
