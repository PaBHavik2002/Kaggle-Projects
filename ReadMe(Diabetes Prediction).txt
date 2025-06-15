# 🧬 Diabetes Prediction – Heart Attack Risk in Germany

## 📌 Project Overview
This project analyzes health and lifestyle data from across Germany to predict the presence of diabetes and explore the relationship with heart attack risk, hypertension, and other contributing factors. A full machine learning pipeline was developed to process 275,000+ records and compare classification model performance.

---

## 📊 Dataset
- Source: Kaggle (Heart Attack in Youth vs Adult – Germany)
- Size: 275,644 rows with 22 features
- Target variable: `Diabetes` (0/1)

---

## 🔍 Exploratory Insights
- **Distribution Analysis**: Visualized histograms, bar charts, and KDE plots for:
  - BMI
  - Alcohol consumption
  - Cholesterol
  - Air pollution
  - Regional heart attack rate
- **Category Balance**: Bar charts showed imbalance in age group (more adults), employment types, and smoking status
- **Chi-Square Tests**: No significant dependency found between hypertension and lifestyle features
- **Pearson Correlation**: Alcohol and cholesterol showed no meaningful correlation (p > 0.05)

---

## 🛠 Machine Learning Pipeline
- One-hot encoded categorical variables (49 total features after encoding)
- Scaled all numerical values
- Addressed target imbalance using **SMOTE (Synthetic Minority Oversampling Technique)**

---

## 🤖 Models Used
- **Logistic Regression**:
  - Accuracy ≈ 63.5%
  - Outperformed Random Forest significantly
- **Random Forest Classifier**:
  - Accuracy ≈ 50.5% (due to overfitting or class imbalance)
  - Tried tuning max depth and estimators

---

## 📈 Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score
- Training vs Test performance compared using line plots
- Logistic regression proved more reliable despite model complexity

---

## 🔄 Improvements Attempted
- GridSearchCV for hyperparameter tuning (not shown in final version)
- Applied SMOTE to resolve class imbalance and avoid biased predictions

---

## 🚀 Future Work
- Train additional classifiers (e.g., Gradient Boosting, SVM)
- Use Deep Neural Networks with sigmoid output layer
- Consider feature selection using mutual information or PCA
- More advanced hyperparameter tuning with randomized search

