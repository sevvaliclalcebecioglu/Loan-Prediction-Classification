# Loan Prediction - Classification Project

## Project Overview
This project focuses on predicting whether a customer will successfully repay a loan. Classification models are used when the output variable is categorical, such as **Yes/No**, **Positive/Negative**, or **Neutral**. Here, the goal is to classify customers into **good credit risk** (likely to repay) or **bad credit risk** (unlikely to repay) based on historical data.

The project demonstrates the complete pipeline for a classification problem, including data preprocessing, feature engineering, model training, evaluation, and feature importance analysis.

---

## Dataset
The dataset contains information about customers and their financial history, including:

- **Credit Score**  
- **Current Loan Amount**  
- **Credit Utilization**  
- **Debt-to-Income Ratio**  
- **Maximum Open Credit**  
- **Monthly Debt**  
- **Years of Credit History**  
- **Current Credit Balance**  
- **Annual Income**  
- **Number of Open Accounts**  
- **Months Since Last Delinquent**  
- **Years in Current Job**  
- **Loan Term (Short/Long)**  
- **Number of Credit Problems**  
- **Purpose of Loan**  

These features are used to train the models to predict loan repayment behavior.

---

## Model Training and Evaluation
Multiple classification models were trained and evaluated using **Accuracy, Precision, Recall, and F1 Score**:

| Model                       | Accuracy  | Precision | Recall   | F1 Score |
|-------------------------------|-----------|-----------|----------|----------|
| **RandomForestClassifier**    | 0.8462    | 0.8462    | 0.8462   | 0.8462   |
| GradientBoostingClassifier    | 0.7646    | 0.7646    | 0.7646   | 0.7646   |
| DecisionTreeClassifier        | 0.7588    | 0.7588    | 0.7588   | 0.7588   |
| AdaBoostClassifier            | 0.7553    | 0.7553    | 0.7553   | 0.7553   |
| LogisticRegression            | 0.7481    | 0.7481    | 0.7481   | 0.7481   |
| KNeighborsClassifier          | 0.7194    | 0.7194    | 0.7194   | 0.7194   |
| BernoulliNB                   | 0.6917    | 0.6917    | 0.6917   | 0.6917   |
| MultinomialNB                 | 0.4482    | 0.4482    | 0.4482   | 0.4482   |

**Key Observation:**  
The **RandomForestClassifier** performed best, achieving approximately **84.6% accuracy**, making it the most reliable model for predicting loan repayment.

---

## Feature Importance
The model identified the most influential features for predicting loan repayment:

| Feature                      | Importance |
|-------------------------------|------------|
| Credit Score                  | 0.1906     |
| Current Loan Amount           | 0.1320     |
| Credit Utilization            | 0.0759     |
| Debt_to_Income                | 0.0725     |
| Maximum Open Credit           | 0.0709     |
| Monthly Debt                  | 0.0685     |
| Years of Credit History       | 0.0684     |
| Current Credit Balance        | 0.0684     |
| Annual Income                 | 0.0586     |
| Number of Open Accounts       | 0.0468     |
| Months Since Last Delinquent  | 0.0414     |
| Years in Current Job          | 0.0318     |
| Loan Term (Short Term)        | 0.0257     |
| Number of Credit Problems     | 0.0070     |
| Purpose (Debt Consolidation)  | 0.0066     |

---

## Critical Questions for Customers
The following questions are derived from the most important features identified by the model. They help collect data for predicting credit risk:

| Feature                      | Question to Ask Customer |
|-------------------------------|------------------------|
| Credit Score                  | What is your credit score? Can you provide an official report? |
| Current Loan Amount           | How much current loan debt do you have? |
| Credit Utilization            | What percentage of your credit card limit are you using? |
| Debt_to_Income                | What is your monthly income and total debt payment? |
| Maximum Open Credit           | What has been your maximum credit limit in the past? |
| Years of Credit History       | How many years of credit history do you have? |
| Current Credit Balance        | What is your current total credit balance? |
| Monthly Debt                  | What is your total monthly debt payment? |
| Annual Income                 | What is your annual income? |
| Number of Open Accounts       | How many credit accounts are currently open? |
| Months Since Last Delinquent  | How many months since your last late payment? |
| Years in Current Job          | How many years have you been in your current job? |
| Loan Term                     | Are you requesting a short-term or long-term loan? |
| Number of Credit Problems     | How many credit problems have you faced previously? |
| Purpose                       | What is the purpose of the loan? |

---

## Conclusion
- The **RandomForestClassifier** is the most effective model for predicting loan repayment, achieving around **85% accuracy**.  
- Critical features such as **Credit Score, Current Loan Amount, Credit Utilization, Debt-to-Income, and Maximum Open Credit** have the highest impact on predictions.  
- The project helps identify good customers efficiently and can support automated credit decision systems.  

---
