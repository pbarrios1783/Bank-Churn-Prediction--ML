# Bank Churn Prediction

### 📌 Overview
This project focuses on predicting customer churn for a bank using machine learning techniques. The objective is to identify customers at risk of leaving and develop strategies to retain them. The notebook explores multiple models and evaluates their performance to choose the best solution for this classification problem.

### 🎯 Objectives
#### Business Goals
Reduce customer churn by identifying high-risk customers.
Provide actionable insights to improve customer retention strategies.

#### Machine Learning Goals
Build and evaluate predictive models to classify customers as likely to churn or remain.
Optimize the model performance using techniques such as hyperparameter tuning, SMOTE, and weighted loss functions.

### 🗂 Dataset
The dataset contains information about bank customers, including demographic, behavioral, and financial details. Key features include:

CustomerID: Unique identifier for each customer.
CreditScore: Customer's credit score.
Geography: Customer's location.
Gender: Gender of the customer.
Age: Customer's age.
Tenure: Number of years the customer has been with the bank.
Balance: Account balance of the customer.
NumOfProducts: Number of products the customer uses.
IsActiveMember: Whether the customer is an active bank member.
EstimatedSalary: Customer's estimated salary.
Exited: Target variable indicating whether the customer churned (1) or remained (0).

### 📋 Notebook Structure
#### 1. Data Preparation
Split the data into training (80%) and testing (20%) subsets.
Preprocess the data:
Handle missing values and encode categorical features.
Scale numerical features.
Address class imbalance using SMOTE and weighted loss functions.

#### 2. Exploratory Data Analysis (EDA)
Visualize the distribution of features and their relationship with the target variable.
Identify patterns and predictors for customer churn.

#### 3. Model Building
Models tested:
Logistic Regression
Random Forest (Tuned and Weighted)
Neural Networks (Two versions: basic and optimized)
Applied hyperparameter tuning and regularization techniques.

#### 4. Model Evaluation
Key metrics used:
Accuracy
Precision
Recall
F1-Score
ROC-AUC
Analysis of false positives and false negatives for business impact.

### ✅ Results
Best Performing Model: Neural Network (Optimized)
Accuracy: 88%
Precision: 85%
Recall: 82%
F1-Score: 83%
ROC-AUC: 0.91

### Key Insights:
Features such as tenure, balance, and transaction frequency were critical predictors of churn.
Addressing class imbalance with SMOTE and weighted loss functions significantly boosted recall.

### 💡 Recommendations
Deploy the optimized Neural Network model for churn prediction.
Integrate the model into the bank’s CRM system to proactively identify and target high-risk customers with retention strategies.
Focus retention efforts on customer segments with high churn risk, such as:
Customers with lower tenure.
Customers with high account balances but low activity.
Retrain and monitor the model periodically with updated data to adapt to changing customer behaviors.

### 🚀 How to Use
Clone this repository:
bash
Copy code
git clone https://github.com/your-repo-name/bank-churn-prediction.git
cd bank-churn-prediction
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Run the notebook in Jupyter or any compatible IDE:
bash
Copy code
jupyter notebook bank-churn-prediction.ipynb

### 📈 Future Work
Incorporate Additional Data: Include more features such as transaction history or customer feedback to improve predictions.
Explainable AI: Use tools like SHAP to explain model predictions to stakeholders.
Test Advanced Models: Experiment with other state-of-the-art algorithms such as XGBoost or AutoML.
