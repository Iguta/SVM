# 🧠 Support Vector Machines (SVM) Project

This project implements Support Vector Machines using Python and scikit-learn to predict whether a loan is **fully paid** or **not fully paid** based on borrower and loan characteristics.

---

## 📂 Project Structure

- `02-Support Vector Machines Project.ipynb` – Main Jupyter Notebook
- `README.md` – Project summary and documentation

---

## 📊 Dataset Overview

The dataset includes features like:

- `credit.policy` – Does the customer meet the credit underwriting criteria?
- `int.rate` – Interest rate of the loan
- `installment` – Monthly payment owed by the borrower
- `log.annual.inc` – Log-transformed annual income
- `purpose` – Purpose of the loan (categorical)
- `fico` – FICO credit score
- `not.fully.paid` – Target variable (1 = Not fully paid, 0 = Fully paid)

---

## 🚀 Workflow Summary

1. **Data Exploration**
   - Identified missing values and categorical features
   - Plotted distributions and relationships

2. **Preprocessing**
   - Created dummy variables for `purpose`
   - Scaled numerical data if needed

3. **Model Training**
   - Used `SVC` from scikit-learn
   - Trained with default and tuned parameters

4. **Evaluation**
   - Used `confusion_matrix` and `classification_report`
   - Compared kernels (e.g., linear, rbf)

---

## 📈 Visualizations

- Countplots by loan status and purpose
- KDE plots for FICO scores
- Confusion matrices
- Jointplots showing interest rate vs. FICO

---

## 🧠 Insights & Observations

- 📉 **FICO Scores Matter** – Higher FICO scores are associated with fewer loan defaults.
- 💸 **Interest Rates** – Defaulted loans tend to have higher interest rates.
- 🎯 **Loan Purpose** – Certain loan types like small business or debt consolidation showed higher default rates.
- 🧪 **Model Findings**:
  - SVM performed well but struggled slightly with class imbalance.
  - RBF kernel handled non-linear boundaries better than linear.
  - Hyperparameter tuning (especially `C` and `gamma`) improves performance.

---

## 📦 Requirements

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
