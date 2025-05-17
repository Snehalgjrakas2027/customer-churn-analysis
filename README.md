# 📊 Customer Churn Prediction Project

This project analyzes customer churn behavior and builds predictive models to identify customers at risk of leaving. It uses data from a telecommunications company and includes data cleaning, exploratory analysis, feature engineering, modeling, and evaluation.

---

## 📁 Project Structure

```
customer-churn-analysis/
│
├── data/
│   ├── WA_Fn-UseC_-Telco-Customer-Churn.csv     # Original dataset
│   └── processed_data.csv                       # Cleaned dataset
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb                   # Data preprocessing and cleaning
│   ├── 02_eda_visualization.ipynb               # Exploratory Data Analysis (EDA)
│   └── 03_modeling.ipynb                        # Model training and evaluation
│
├── scripts/
│   └── churn_prediction.py                      # Model training script (Python script version)
│
├── plots/
│   ├── churn_distribution.png
│   ├── contract_vs_churn.png
│   ├── roc_curve.png
│   └── confusion_matrix.png
│
├── README.md                                     # Project documentation
└── requirements.txt                              # List of required packages
```

---

## 🧾 Dataset

* **Source**: [Telco Customer Churn dataset (IBM Sample)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
* **Description**: The dataset contains information about a telecom company's customers including demographic, service usage, and billing data.
* **Target Variable**: `Churn` — whether the customer left the company (Yes/No)

---

## ✅ Project Goals

### Phase 1–2: Data Cleaning

* Handle missing values and data types
* Convert categorical values
* Save cleaned data for future use

### Phase 3: Exploratory Data Analysis (EDA)

* Analyze churn by tenure, contract type, payment method, etc.
* Visualize data using seaborn and matplotlib (bar plots, box plots, histograms)
* Generate a correlation heatmap
* Conduct basic statistical tests (chi-square, t-test)

### Phase 4: Modeling

* Feature engineering (encoding, scaling)
* Train models: Logistic Regression, Random Forest
* Evaluate using Accuracy, Precision, Recall, ROC AUC
* Visualize ROC curve and confusion matrix
* Explain feature importance

---

## 🔍 Key Findings

* Customers with **month-to-month contracts** and **electronic check payments** had higher churn rates.
* Longer-tenured customers were less likely to churn.
* **TotalCharges**, **tenure**, and **contract type** were among the most important features in predicting churn.

---

## 🧠 Models Used

| Model               | Accuracy  | Precision | Recall   | ROC AUC    |
| ------------------- | --------- | --------- | -------- | ---------- |
| Logistic Regression | \~80%     | Moderate  | Moderate | \~0.83     |
| Random Forest       | **\~82%** | High      | High     | **\~0.86** |

---

## 📈 Visualizations

* Churn distribution
* Churn by contract type
* Boxplots of tenure and monthly charges by churn
* ROC Curve and confusion matrix

*Screenshots of plots can be found in the `/plots` folder.*

---

## 🚀 How to Run

### Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

### Run Notebooks

Use Jupyter or VS Code to open and run the following:

1. `notebooks/01_data_cleaning.ipynb`
2. `notebooks/02_eda_visualization.ipynb`
3. `notebooks/03_modeling.ipynb`

### Run Model Script (optional)

```bash
python scripts/churn_prediction.py
```

---

## 📚 Requirements

Key libraries used:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `scipy`

*All libraries listed in `requirements.txt`.*

---

## 📌 Future Improvements

* Deploy model using Flask or Streamlit
* Implement automated retraining with new data
* Hyperparameter tuning with GridSearchCV or Optuna

---

## 🧑‍💻 Author

* **Your Name**
  GitHub Profile: https://github.com/Snehalgjrakas2027
  📫 Email: snehalgjrakas118@gmail.com

---

Let me know if you'd like this exported as a file or customized further with your name, screenshots, or links!
