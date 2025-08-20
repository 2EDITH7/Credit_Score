# Credit Risk Prediction using Machine Learning

## 📌 Overview
This project predicts whether a customer will **default on a loan** using the [Kaggle Credit Risk Dataset](https://www.kaggle.com/datasets/laotse/credit-risk-dataset).  
We apply **Exploratory Data Analysis (EDA)** and train **Logistic Regression** and **Random Forest** models to classify credit risk.

---

## 📊 Dataset
The dataset includes records of **10,000+ customers**, with features such as:
- Demographics: age, income, home ownership, employment length
- Loan details: loan amount, interest rate, loan percent income (utilization ratio)
- Credit history: previous defaults (proxy for payment history)
- Target: loan_status (1 = default, 0 = repaid)

---

## 🔎 Methodology
1. **Data Preprocessing**  
   - Missing value handling  
   - Encoding categorical variables  
   - Standardization  

2. **EDA**  
   - Utilization ratio vs default  
   - Payment history vs default  
   - Age & income analysis  

3. **Models Used**  
   - Logistic Regression  
   - Random Forest  

4. **Evaluation Metrics**  
   - Confusion Matrix  
   - Precision, Recall, F1-score  
   - ROC-AUC Curve  

---

## 📈 Results
- Logistic Regression ROC-AUC: ~0.75  
- Random Forest ROC-AUC: ~0.85–0.90  
- Key predictors:  
  - Loan percent income (utilization ratio)  
  - Previous defaults (payment history)  
  - Borrower income  
  - Age  

---

## 📂 Repository Structure
```
credit-risk-prediction/
│── data/               # Dataset
│── notebooks/          # Jupyter notebooks for EDA & Modeling
│── src/                # Python scripts
│── results/            # Graphs & model performance
│── report/             # Academic report
│── README.md           # Project overview
│── requirements.txt    # Dependencies
```

---

## ⚙️ Installation & Usage
```bash
# Clone repo
git clone https://github.com/your-username/credit-risk-prediction.git
cd credit-risk-prediction

# Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook
```

---

## 📜 License
This project is licensed under the **MIT License**.

---

### requirements.txt
```
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

### report/academic_report.md

# Credit Risk Prediction Project Report

## 1. Introduction
Credit scoring is an essential tool for assessing borrowers’ repayment ability. Using the Kaggle Credit Risk Dataset, we analyze over 10,000 records to identify factors influencing defaults and build predictive models.

## 2. Methodology
- Preprocessing: handled missing values, encoded categorical features, and standardized numeric data.
- EDA: analyzed utilization ratio (`loan_percent_income`), payment history, age, and income.
- Models: Logistic Regression & Random Forest trained and evaluated.

## 3. Results
- Logistic Regression AUC ≈ 0.75
- Random Forest AUC ≈ 0.85–0.90
- Key features: loan percent income, previous defaults, income, age.

## 4. Conclusion
Random Forest outperformed Logistic Regression in credit risk prediction. Utilization ratio and payment history were found to be the most critical factors in default prediction. These models can be applied in finance and beyond (insurance, telecom, e-commerce).

---

