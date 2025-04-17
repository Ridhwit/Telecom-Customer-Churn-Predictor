# 📞 Telecom Customer Churn Predictor

## 📌 Project Overview
The Telecom Customer Churn Predictor is a machine learning-based solution that identifies customers who are likely to leave a telecom service provider. By leveraging customer data such as tenure, charges, contract type, and demographic details, the model helps telecom companies take proactive measures to reduce churn and improve customer retention.

## 🧠 Model Overview
This project uses a **Random Forest Classifier** trained on telecom customer data. To enhance prediction accuracy and handle class imbalance, we employed **SMOTEENN**(Synthetic Minority Over-sampling Technique with Edited Nearest Neighbors) which is a hybrid of oversampling and cleaning techniques. 

## 🌟 Key Features
- Predicts whether a customer is likely to churn based on inputs.
- Handles imbalanced datasets with **SMOTEENN** resampling.
- Accepts key customer features like tenure, charges, contract type, etc.
- Outputs churn prediction in real time.

## 📊 Model Performance
**Before SMOTEENN:**
- Accuracy: **80.02%**
- Precision (Churn): 0.69
- Recall (Churn): 0.45
- F1-score (Churn): 0.54

**After SMOTEENN:**
- Accuracy: **93.57%**
- Precision (Churn): 0.92
- Recall (Churn): 0.97
- F1-score (Churn): 0.94
By applying SMOTEENN, the model's performance improved drastically, particularly in predicting the minority class (churn), leading to better recall and more accurate results.

Confusion Matrix:


## 🎯 Business Objective
Customer churn prediction is crucial for telecom companies to:

- Identify high-risk customers and proactively intervene to retain them.
- Minimize customer attrition by offering personalized incentives and services.
- Improve customer satisfaction and loyalty by addressing issues before they lead to churn.

## 📈 Output & Impact
- **Output**: Predicts whether a given customer is likely to churn.
- **Impact**: Helps the company take preemptive action, reduce customer loss, and boost overall customer satisfaction.

## 🔮 Future Objectives
- Add more customer features to improve model performance.
- Integrate customer interaction history or service complaints.
- Deploy the model with a backend API for real-time production use.
- The model can be further improved by incorporating additional features such as customer complaints, network issues, and more advanced machine learning techniques (e.g., XGBoost, LightGBM).

## ⚙️ How the Model is Working

![image](https://github.com/user-attachments/assets/3a9f7104-608e-4788-86bc-6aba0d73710a)

![image](https://github.com/user-attachments/assets/7cfb794d-1b18-4a59-b75a-f07605dbacfc)

Users input customer details like tenure, contract type, charges, etc. The app transforms this input to match the original model features and makes a prediction using the trained `RandomForestClassifier`. The result is shown instantly as either **"Churn"** or **"No Churn"**.

## 🛠️ Technologies Used
- **Python**
- **Pandas**
- **Scikit-learn**
- **Imbalanced-learn (SMOTEENN)**
- **Streamlit**
- **Joblib**
- **Jupyter Notebook**

---

