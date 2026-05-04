# 📊 Financial Inclusion in East Africa

A machine learning project exploring the factors influencing financial inclusion across East Africa and predicting the likelihood of individuals having a bank account.

🔗 Live App: https://financial-inclusion-east-africa.streamlit.app/

---

**Problem Statement**

Financial inclusion remains a key challenge across East Africa, where access to formal banking services is uneven across different demographic and socioeconomic groups.

Understanding who is more likely to own or use a bank account can help inform policies, improve financial access, and guide digital banking solutions.

---

**Objective**

This project aims to:
- Identify key factors influencing financial inclusion  
- Explore patterns across countries, demographics, and socioeconomic variables  
- Build a machine learning model to predict the likelihood of an individual having a bank account  

---

**Dataset Overview**

The dataset contains demographic and socioeconomic data for individuals across:
- Kenya  
- Uganda  
- Tanzania  
- Rwanda  

spanning the years **2016 to 2018**.

---

**Key Insights**

- Financial inclusion increases with education level and age  
- Access to a mobile phone is strongly associated with having a bank account  
- Urban populations show higher inclusion compared to rural populations  
- The dataset is imbalanced, with a majority of individuals not having bank accounts  

---

**Modeling Approach**

- Outliers were handled using the IQR method with domain constraints  
- Categorical variables were encoded using label encoding, one-hot encoding, and ordinal mapping  
- Class imbalance was addressed using SMOTE on the training data  
- A Random Forest classifier was trained and optimized using Randomized Search  

---

**Model Performance**

- The model achieves strong overall accuracy on the test set  
- Performance on the minority class remains more challenging due to class imbalance  
- Evaluation includes precision, recall, and F1-score to better assess model performance  

---

**Deployment**

- The model and preprocessing pipeline were saved using `joblib`  
- A Streamlit application was built for interactive predictions  
- The app ensures consistent preprocessing between training and inference  

---

**Tech Stack**

- Python  
- Pandas & NumPy  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  
- Streamlit  

---

**Project Structure**
```

financial_inclusion_East_Africa/
├── data/
├── app.py
├── model.pkl
├── preprocessing_artifacts.pkl
├── requirements.txt
├── financial_inclusion.html
├── financial_inclusion_EA.ipynb
└── README.md

```
---

**Future Improvements**

- Improve performance on the minority class  
- Explore additional models and ensemble methods  
- Incorporate more granular economic and geographic data  

---

**Conclusion**

This project demonstrates an end-to-end machine learning workflow, from data exploration and feature engineering to model training, evaluation, and deployment.
