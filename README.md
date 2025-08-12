📌 Overview
This project is a Machine Learning application that predicts whether a loan can be sanctioned based on applicant information.
It uses Random Forest Classifier for prediction and a Streamlit web interface for user interaction.

📂 Project Structure

Loan_Prediction_Classification_Project/


├── cleaned_str.csv           # Cleaned dataset after preprocessing

├── frontend.py               # Streamlit web application

├── loan_prediction.csv       # Original dataset

├── model.ipynb               # Jupyter Notebook for data preprocessing & model training

├── rfmodel.pkl               # Saved Random Forest model

📊 Dataset Information

Target Variable:

loan_status

1 → Loan can be sanctioned

0 → Loan cannot be sanctioned

Features:

Feature	Description


person_age	Applicant’s age

person_gender	Gender

person_education	Education level

person_income	Annual income

person_emp_exp	Employment experience (years)

person_home_ownership	Home ownership type

loan_amnt	Loan amount requested

loan_intent	Loan purpose

loan_int_rate	Loan interest rate

loan_percent_income	Loan amount as % of income

cb_person_cred_hist_length	Credit history length (years)

credit_score	Applicant’s credit score

previous_loan_defaults_on_file	Previous defaults (Yes/No)

🛠 Technologies Used
Python

Pandas, NumPy — Data manipulation

Matplotlib, Seaborn — Visualization

Scikit-learn — Model training

Streamlit — Web application

Pickle — Model saving/loading

🔍 Model Development
Two models were trained:

SVM (RBF Kernel) — Accuracy: ~71%

Random Forest Classifier — Accuracy: ~88% (selected model)

Random Forest Parameters:


RandomForestClassifier(
    n_estimators=150,
    max_depth=5,
    random_state=42
)
Performance:

Training Accuracy: 89%

Testing Accuracy: 88%

💻 How to Use the App

Open the app in your browser (default: http://localhost:8501)

Enter all applicant details in the form

Click Submit

The model will display the prediction:

Loan can be sanctioned

Loan cannot be sanctioned

📜 License
This project is created for educational purposes.
