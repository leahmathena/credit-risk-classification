**Module 12 Report** 

---

# **Credit Risk Classification Report**

## **Overview of the Analysis**
This project focuses on building a **machine learning model** to assess credit risk. The goal is to predict whether a loan is **healthy (0)** or **high-risk (1)** based on various financial indicators. This analysis is essential for **financial institutions** to manage lending risk and make informed decisions.

### **Data Used**
The dataset contains **77,536 loan records** with the following key financial features:
- **Loan Size** – The amount borrowed.
- **Interest Rate** – The percentage rate charged on the loan.
- **Borrower Income** – The borrower's annual income.
- **Debt-to-Income Ratio** – Total debt compared to income.
- **Number of Accounts** – The number of credit accounts the borrower has.
- **Derogatory Marks** – Negative marks on the borrower's credit history.
- **Total Debt** – The total outstanding debt of the borrower.
- **Loan Status** – The **target variable (0 = healthy loan, 1 = high-risk loan)**.

### **Machine Learning Process**
1. **Data Preparation:**
   - Loaded the dataset and explored its structure.
   - Separated the data into **features (X)** and **target variable (y)**.
   - Performed a **train-test split (80% training, 20% testing).**

2. **Model Selection & Training:**
   - Used **Logistic Regression**, a common classification algorithm for binary outcomes.
   - Fitted the model using the **training data**.

3. **Model Evaluation:**
   - Used a **confusion matrix** to evaluate correct and incorrect predictions.
   - Generated a **classification report** to assess **precision, recall, and F1-score**.

---

## **Results**

### **Machine Learning Model: Logistic Regression**
- **Accuracy:** **99%**
- **Precision (Healthy Loan - 0):** **1.00**
- **Recall (Healthy Loan - 0):** **1.00**
- **F1-Score (Healthy Loan - 0):** **1.00**
- **Precision (High-Risk Loan - 1):** **0.89**
- **Recall (High-Risk Loan - 1):** **0.92**
- **F1-Score (High-Risk Loan - 1):** **0.91**

---

## **Summary & Recommendation**
The **Logistic Regression model performed extremely well**, achieving a **99% accuracy rate**. The model **perfectly predicts healthy loans (0)** and does a strong job at identifying **high-risk loans (1)** with **92% recall**. However, **11% of healthy loans are incorrectly flagged as high-risk**, which could result in unnecessary loan rejections.

### **Recommendation:**
- If the company **prioritizes minimizing loan default risk**, this model is **recommended** since it correctly identifies most high-risk loans.
- If the company **wants to reduce false high-risk classifications**, further tuning or alternative models might be necessary.

Overall, this **Logistic Regression model is a strong candidate for credit risk assessment**, providing a reliable tool for managing loan decisions.

---

**Project by: Leah Mathena**  
