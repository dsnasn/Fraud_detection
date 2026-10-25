
# 💳 Financial Fraud Detection Using Machine Learning

An end-to-end financial fraud detection project using **Python, SQL, DuckDB, and Machine Learning** on the PaySim synthetic financial dataset.

This project explores fraudulent transaction patterns through SQL-based exploratory data analysis (EDA), data preprocessing, feature engineering, machine learning classification, and model explainability.

The primary focus is on identifying fraudulent financial transactions in highly imbalanced data.

---

## 🎯 Project Objectives

- Analyse financial transaction patterns using SQL and Python.
- Identify key characteristics of fraudulent transactions.
- Perform exploratory data analysis (EDA) and feature engineering.
- Investigate class imbalance and its impact on fraud detection.
- Explore machine learning models for fraud classification.
- Evaluate model performance using appropriate classification metrics.
- Investigate feature importance and model interpretability.

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| Programming | Python, SQL |
| Data Analysis | Pandas, NumPy, DuckDB |
| Machine Learning | Scikit-learn, XGBoost |
| Model Explainability | SHAP |
| Data Visualization | Matplotlib |
| Development Environment | Jupyter Notebook |

---

## 📂 Project Structure

```text
Fraud_detection/
│
├── PaySim_FraudDetection_Project.ipynb  # Machine Learning & Fraud Detection
├── PaySim_SQL_EDA_DuckDB.ipynb          # SQL-based Exploratory Data Analysis
├── requirements.txt                     # Python Dependencies
└── README.md                            # Project Documentation
```

**Note:** The dataset is not included in this GitHub repository due to its large file size. It must be downloaded separately from Kaggle.

---

## 📊 Dataset

This project uses the **PaySim Synthetic Financial Dataset**, which simulates mobile money transactions and contains both legitimate and fraudulent activities.

The dataset consists of approximately **6.36 million transactions** with the following features:

| Feature | Description |
|---------|-------------|
| step | Transaction time step |
| type | Transaction type (CASH_IN, CASH_OUT, DEBIT, PAYMENT, TRANSFER) |
| amount | Transaction amount |
| nameOrig | Originating account |
| oldbalanceOrg | Sender's balance before the transaction |
| newbalanceOrig | Sender's balance after the transaction |
| nameDest | Destination account |
| oldbalanceDest | Recipient's balance before the transaction |
| newbalanceDest | Recipient's balance after the transaction |
| isFraud | Fraud classification label |
| isFlaggedFraud | Flag indicating potentially fraudulent transfers |

**Dataset Source:**

[PaySim Synthetic Financial Dataset – Kaggle](https://www.kaggle.com/datasets/ealaxi/paysim1?resource=download)

### ⚠️ Dataset Download Required

The dataset is **NOT included in this GitHub repository** due to its large file size.

To reproduce the analysis:

1. Visit the [PaySim Kaggle Dataset](https://www.kaggle.com/datasets/ealaxi/paysim1?resource=download).
2. Download and extract the dataset.
3. Rename the extracted CSV file to `paysim_dataset.csv`.
4. Place the CSV file in the project root directory.
5. Ensure the dataset path in the notebooks points to `paysim_dataset.csv`.

**Expected local directory structure:**

```text
Fraud_detection/
│
├── PaySim_FraudDetection_Project.ipynb
├── PaySim_SQL_EDA_DuckDB.ipynb
├── paysim_dataset.csv
├── requirements.txt
└── README.md
```

The CSV file is required to run the analysis and train the machine learning models.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/dsnasn/Fraud_detection.git
cd Fraud_detection
```

### 2. Create a Virtual Environment

Python 3.11 is recommended for compatibility with the machine learning libraries.

**macOS / Linux:**

```bash
python3.11 -m venv env
source env/bin/activate
```

**Windows:**

```bash
python -m venv env
env\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the Dataset

Download the PaySim dataset from Kaggle:

https://www.kaggle.com/datasets/ealaxi/paysim1?resource=download

Extract the CSV file, rename it to `paysim_dataset.csv`, and place it in the project directory.

### 5. Run the Jupyter Notebooks

Open the notebooks in Jupyter Notebook or Visual Studio Code.

To launch Jupyter Notebook:

```bash
jupyter notebook
```

Ensure the correct Python environment is selected.

**Recommended execution order:**

1. `PaySim_SQL_EDA_DuckDB.ipynb` — SQL-based data exploration.
2. `PaySim_FraudDetection_Project.ipynb` — Machine learning and fraud detection.

---

## 🔍 Project Workflow

### 1. SQL-Based Exploratory Data Analysis

**Notebook:** `PaySim_SQL_EDA_DuckDB.ipynb`

Explore financial transaction data using SQL queries executed through DuckDB.

Key areas of analysis:

- Transaction volume and distribution.
- Fraudulent vs legitimate transactions.
- Fraud patterns across transaction types.
- Transaction amount analysis.
- Account balance behaviour.
- Data quality and consistency checks.

### 2. Data Preprocessing & Feature Engineering

**Notebook:** `PaySim_FraudDetection_Project.ipynb`

Prepare the dataset for machine learning:

- Handle missing values and data quality issues.
- Encode categorical variables.
- Select and engineer relevant transaction features.
- Split the dataset into training and testing sets.
- Investigate strategies for handling class imbalance.

### 3. Machine Learning Model Development

Explore fraud classification using machine learning algorithms, including:

- Scikit-learn classification models.
- XGBoost.

The objective is to distinguish fraudulent transactions from legitimate transactions while addressing the challenges of imbalanced classification.

### 4. Model Evaluation

Evaluate model performance using:

- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

Because fraudulent transactions account for a very small proportion of the dataset, **Precision and Recall are particularly important**, rather than relying solely on classification accuracy.

### 5. Model Explainability

Explore model interpretability using:

- Feature Importance
- SHAP (SHapley Additive exPlanations)

These techniques can help identify which transaction features contribute most significantly to fraud predictions.

---

## 📈 Future Improvements

- Experiment with additional machine learning algorithms.
- Improve classification performance through hyperparameter tuning.
- Explore advanced class imbalance handling techniques.
- Enhance feature engineering and model explainability.
- Investigate model deployment and real-time fraud detection.

---

## 📚 References

**PaySim Dataset**

Lopez-Rojas, E. A., Elmir, A., & Axelsson, S. (2016).

*PaySim: A Financial Mobile Money Simulator for Fraud Detection.*

Dataset available at:

https://www.kaggle.com/datasets/ealaxi/paysim1?resource=download

---

## 👩‍💻 Author

**Jiahui (Katie) Ma**

Operations Analyst @ Barclays | MSc Computing Science, University of Glasgow

Interested in Data Science, Machine Learning, Artificial Intelligence, and technology-driven problem solving.

- **GitHub:** [dsnasn](https://github.com/dsnasn)
- **LinkedIn:** [Jiahui Ma](https://linkedin.com/in/jiahui-ma-b57b56337)

---

⭐ *Continuously learning, experimenting, and exploring real-world applications of Machine Learning and AI.*
