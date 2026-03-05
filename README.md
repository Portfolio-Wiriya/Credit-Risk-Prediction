# Credit Risk Prediction Projrct  for Loan Default

## Project Overvire

This project to predict the probability of credit card default using machine learning.
การประเมินความเสี่ยงของลูกค้าที่ต้องการทำการกู้ยืมสินเชื่อ ว่ามีความเสี่ยงที่จะชำระหนี้หรือไม่ชำระหนี้หรือไม่ 
เพื่อลดความเสี่ยงของธนาคารที่จะเจอลูกค้าค้างชำระค่าสินเชื่อ เป็นตัวช่วยในการทำนายว่าผู้ใดมีความเสี่ยงในการค้างค่าชำระน้อยที่สุด เพื่อง่ายต่อการอนุมัติการกู้ยืม
โปรเจคนี้มีการใช้ Data cleaning, Data analysis, Machine learning model, and risk scoring


## Business Problem
ธนาคารมีความเสี่ยงที่ลูกค้าจะผิดนัดชำระหนี้
หากมีการผิดนัดชำระหนี้ ผลที่ตามมีคือธนาคารไม่ได้รับค่าชำระตามเวลาที่กำหนดทำให้เกิดปัญหาทางด้านการขาดทุนของธนาคาร

การแก้ปัญหาคือการคัดกรองลูกค้าที่ต้องการทำสินเชื่อตั้งแต่เริ่มต้น เพื่อลดความเสี่ยงในการเกิดการค้างชำระหนี้

This allows financial institutions to:

- Identify high-risk customers
- Improve credit approval decisions
- Reduce financial losses from defaults

## Dataset
The dataset contains credit card customer information including demographic data, payment history, bill amounts, and repayment behavior.

Key features include:

- LIMIT_BAL : Credit limit
- SEX : Gender
- EDUCATION : Education level
- MARRIAGE : Marital status
- AGE : Customer age
- PAY_0 - PAY_6 : Payment status history
- BILL_AMT : Bill statement amounts
- PAY_AMT : Previous payments

Target variable:

- default : Whether the customer defaulted on their credit payment

## Project Workflow

The project follows a standard data science pipeline:

1. Data Cleaning
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Model Training
5. Model Evaluation
6. Risk Scoring


## Exploratory Data Analysis 

insight ที่เจอ

Key findings from the data analysis:

- Customers with late payment history have a significantly higher default rate.
- High credit utilization is associated with higher default risk.
- Younger customers tend to have slightly higher default probabilities.

## Model Development

Several machine learning models were tested:

- Logistic Regression
- Random Forest
- XGBoost

Evaluation metrics used:

- Accuracy
- Precision
- Recall
- ROC-AUC

The Random Forest model achieved the best performance in predicting default risk.

## Results

Model performance:

Accuracy : 0.82  
Precision : 0.79  
Recall : 0.75  
ROC-AUC : 0.86

Important features influencing default prediction:

- Payment status history
- Credit utilization
- Credit limit

## Tech Stack

Programming Language
- Python

Libraries
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

Tools
- Jupyter Notebook
- Git
- GitHub

## Project Structure

credit-risk-project
│
├── data
│
├── notebooks
│   └── EDA.ipynb
│
├── src
│   ├── data_cleaning.py
│   ├── feature_engineering.py
│   ├── train_model.py
│
└── README.md

## Future Improvements

Possible improvements for this project:

- Implement real-time prediction API
- Deploy the model using FastAPI
- Build a dashboard for risk monitoring
- Improve model performance using advanced ensemble techniques
