# 🧠 Support Vector Machines (SVM) Project

This project demonstrates the implementation of **Support Vector Machines (SVM)** using Python and `scikit-learn` for binary classification. The dataset includes loan application data, and the goal is to predict whether a loan was **fully paid** or **not fully paid**.

---

## 📁 Project Structure

- `02-Support Vector Machines Project.ipynb`: Jupyter notebook containing the full analysis, model training, and evaluation.
- `README.md`: Project overview and setup instructions.

---

## 📊 Dataset Description

The dataset contains the following key columns:

- `credit.policy`
- `int.rate`
- `installment`
- `log.annual.inc`
- `purpose` *(categorical)*
- `fico`
- `days.with.cr.line`
- `revol.bal`
- `revol.util`
- `inq.last.6mths`
- `delinq.2yrs`
- `pub.rec`
- `not.fully.paid` *(target variable)*

---

## 🚀 Workflow Summary

1. **Exploratory Data Analysis (EDA)**
   - Checked for missing values and data distribution
   - Used `seaborn` and `matplotlib` for visualization

2. **Data Preprocessing**
   - Converted the `purpose` column to dummy variables using `pd.get_dummies()`
   - Dropped the first dummy variable to avoid multicollinearity (`drop_first=True`)
   - Prepared the final feature set

3. **Train/Test Split**
   - Used `train_test_split` from `sklearn.model_selection` to split data into training and testing sets

4. **Model Training**
   - Trained a Support Vector Classifier using `SVC()` from `sklearn.svm`
   - Tried different kernels: `linear`, `rbf`, etc.
   - Adjusted hyperparameters like `C` and `gamma`

5. **Model Evaluation**
   - Evaluated performance using:
     - Confusion Matrix
     - Classification Report
   - Assessed accuracy, precision, recall, and F1-score

---

## 📈 Visualizations

- Confusion matrix heatmap
- KDE and scatter plots using Seaborn’s `FacetGrid`
- Count plots and pair plots for feature distribution

---

## 📌 Dependencies

Install with:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
