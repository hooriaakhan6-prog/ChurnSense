<div align="center">

# 🔮 ChurnSense
### *Know Who's Leaving — Before They Do*

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)](https://spark.apache.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

[![Status](https://img.shields.io/badge/Status-Complete-00C853?style=flat-square)]()
[![License](https://img.shields.io/badge/License-MIT-blueviolet?style=flat-square)]()


<br/>

> 💡 *Businesses lose billions every year to customer churn.*
> *ChurnSense uses machine learning to detect at-risk customers — before it's too late.*

<br/>

---

</div>

## 🧠 What is ChurnSense?

**ChurnSense** is an end-to-end machine learning pipeline that predicts **customer churn** for a telecom company. Built on real-world Kaggle data, it identifies customers who are likely to cancel their subscription — giving businesses the chance to **act proactively and retain revenue.**

```
Customer Data  ──►  Cleaning  ──►  EDA  ──►  Feature Eng.  ──►  ML Model  ──►  Churn Prediction ✅
```

---

## 🎯 Objectives

- 🔍 Uncover hidden churn patterns through deep EDA
- 🧹 Clean and preprocess messy real-world telecom data
- ⚙️ Engineer meaningful features for better model performance
- 🤖 Train & compare multiple classification models
- 📊 Evaluate models with industry-standard metrics

---

## 📂 Dataset — Telco Customer Churn (Kaggle)

| Property | Detail |
|----------|--------|
| 📦 Source | [Kaggle — Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) |
| 👥 Records | 7,043 customers |
| 🧮 Features | 21 columns |
| 🎯 Target | `Churn` → Yes / No |

**Key feature categories:**

```
👤 Demographics     →  gender, age, dependents, partner
📋 Account Info     →  tenure, contract type, payment method
🌐 Services Used    →  internet, phone, streaming, security
💳 Billing Details  →  monthly charges, total charges
🎯 Target Variable  →  Churn (Yes / No)
```

---

## 🛠️ Tech Stack

| Layer | Tools |
|-------|-------|
| 🐍 Language | Python 3.8+ |
| ⚡ Big Data | PySpark, PySpark MLlib |
| 📊 Analysis | Pandas, NumPy |
| 📈 Visualization | Matplotlib, Seaborn |
| 🤖 ML Models | Scikit-learn, PySpark MLlib |
| 📓 Environment | Jupyter Notebook |

---

## 🔍 Data Preprocessing

- ✅ Handled missing & null values
- ✅ Converted `TotalCharges` from string → numeric
- ✅ Encoded categorical variables (`StringIndexer`, `OneHotEncoder`)
- ✅ Feature scaling for model compatibility
- ✅ Assembled feature vectors using `VectorAssembler`

---

## 📊 Exploratory Data Analysis

Uncovered critical business insights, including:

- 📉 **~26% of customers churned** — significant class imbalance
- 📆 Customers on **month-to-month contracts** churn the most
- 💸 High **monthly charges** strongly correlate with churn
- 🕐 **New customers (low tenure)** are at highest risk
- 🔒 Add-on services (security, backup) **reduce churn likelihood**

---

## 🤖 Machine Learning Models

Three classifiers were trained and compared:

| Model | Type | Library |
|-------|------|---------|
| 🔵 Logistic Regression | Linear | PySpark MLlib |
| 🌳 Decision Tree | Tree-based | Scikit-learn |
| 🌲 Random Forest | Ensemble | Scikit-learn |

**Train/Test Split:** 80% / 20%

---

## 📈 Model Evaluation

Models evaluated using:

| Metric | Description |
|--------|-------------|
| ✅ Accuracy | Overall correct predictions |
| 📊 Confusion Matrix | True/False Positives & Negatives |
| 🎯 Precision | How many predicted churners actually churned |
| 🔁 Recall | How many actual churners were caught |
| 📉 AUC-ROC | Model's ability to distinguish classes |

> 🏆 **Best performing model:** Logistic Regression — ~80% Accuracy | AUC ~0.84
> *(Update with your actual scores from the notebook!)*

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Java 8+ *(required for PySpark)*

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/hooriaakhan6-prog/ChurnSense.git
cd ChurnSense
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Launch the Notebook

```bash
jupyter notebook churnsense.ipynb
```

---

## 📁 Project Structure

```
📦 ChurnSense/
 ┣ 📓 churnsense.ipynb       ← Full ML pipeline notebook
 ┣ 📜 requirements.txt       ← All dependencies
 ┣ 📄 README.md              ← You're here!
 ┗ 🚫 .gitignore             ← Ignored files
```

---

## 📦 requirements.txt

```
pyspark
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

## 💡 Future Roadmap

- [ ] 🔧 Hyperparameter tuning with `CrossValidator`
- [ ] ⚖️ Handle class imbalance with SMOTE
- [ ] 🌐 Deploy as REST API using Flask or FastAPI
- [ ] 📊 Build interactive dashboard with Streamlit
- [ ] 🧠 Experiment with XGBoost and Neural Networks
- [ ] ☁️ Scale pipeline on AWS EMR or Databricks

---

## 👩‍💻 Author

<div align="center">

**Hooria Khan**
*Aspiring Data Engineer | ML Enthusiast | Data Science Graduate*

[![GitHub](https://img.shields.io/badge/GitHub-hooriaakhan6--prog-181717?style=for-the-badge&logo=github)](https://github.com/hooriaakhan6-prog)

</div>

---

<div align="center">

### ⭐ If ChurnSense helped or impressed you — drop a star!


---

*Built with  Python, and way too much ☕ — ChurnSense © 2026*

</div>
