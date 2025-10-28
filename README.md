🏦 Bank Marketing Campaign Analysis and Term Deposit Prediction

Predicting term deposit subscriptions using data from a Portuguese bank’s marketing campaigns.
This project includes data cleaning, exploratory data analysis (EDA), and predictive modeling using Logistic Regression and Random Forest to identify key factors influencing customer conversion rates.

📁 Dataset

Source: Kaggle - Bank Marketing Dataset

Records: 11,162

Features: 17


⚙️ Project Workflow
1. Data Preparation

Downloaded dataset using KaggleHub.

Cleaned and normalized categorical values.

Replaced “unknown” entries with “other” for categorical consistency.

Checked for missing data and validated data integrity.

2. Exploratory Data Analysis (EDA)

Examined feature distributions (age, balance, duration, campaign, etc.).

Correlation analysis for numeric variables.

Visualized conversion rates by job, education, marital status, contact type, and month.

3. Data Preprocessing

Applied One-Hot Encoding for categorical columns.

Standardized numeric columns using StandardScaler.

Split data into Training (80%) and Testing (20%) sets.

4. Model Building

Implemented and compared two supervised classification models:

Logistic Regression

Random Forest Classifier

Both models were built within Scikit-learn Pipelines for clean, reproducible preprocessing and modeling.

5. Evaluation Metrics

Accuracy

ROC-AUC Score

Precision / Recall / F1-Score

Confusion Matrix

Feature Importance & Coefficients

📊 Results
Model	Accuracy	ROC-AUC
Logistic Regression	0.83	0.91
Random Forest	0.85	0.918

Random Forest slightly outperformed Logistic Regression in both accuracy and AUC.

The most influential feature for both models was duration, followed by poutcome_success, and contact_type.

🧠 Key Insights

Longer call durations and successful past marketing outcomes significantly increased conversion likelihood.

Students and retired clients showed higher conversion rates.

Clients contacted via cellular performed better than other contact types.

May had the lowest conversion rate; December and March were the highest.

🚀 Tech Stack

Python 3.x

Libraries: pandas, numpy, seaborn, matplotlib, scikit-learn, kagglehub

Environment: Google Colab

🗂️ Repository Structure
Bank-Marketing-Campaign-Analysis-and-Term-Deposit-Prediction/
│
├── Bank_Marketing_Analysis.ipynb       # Main analysis notebook
├── README.md                           # Project documentation
├── requirements.txt                    # Dependencies
└── dataset/                            # Contains bank.csv


🧩 Future Improvements

Implement hyperparameter tuning (GridSearchCV).

Explore gradient boosting models (XGBoost, LightGBM).

Deploy using Streamlit for interactive predictions.

✍️ Author

Vihar Dilip Yeole
Mail: viharyeole@gmailcom  
Linkedin: https://www.linkedin.com/in/viharyeole/
