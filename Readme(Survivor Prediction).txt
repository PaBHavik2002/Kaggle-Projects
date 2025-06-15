# 🚀 Survivor Prediction – Spaceship Titanic

## 📌 Project Overview
This project predicts whether a passenger was transported to an alternate dimension in the fictional "Spaceship Titanic" dataset. Using advanced feature engineering, data transformation, and classification models like Random Forest, SVM, and XGBoost, we classify passenger survival (transportation) status with a focus on accuracy, model evaluation, and pipeline optimization.

---

## 📊 Dataset
- Source: Kaggle (Spaceship Titanic)
- Size: 8,514 training rows and 4,277 test rows
- Target variable: `Transported` (True/False)

---

## 🔧 Key Features Engineered
- **Total Bill Paid**: Combined expenditure across Spa, FoodCourt, VRDeck, etc.
- **NoExpense**: Binary indicator for passengers with zero expenditure.
- **Passenger ID Parsing**: Splitting passenger groups for more granular insights.
- **Cabin Components**: Extracted deck, number, and side from cabin data.

---

## 🧪 Data Preprocessing
- Imputed missing numerical values using interpolation.
- Filled categorical values with mode.
- One-hot encoding of all categorical variables.
- Scaled numerical data using `StandardScaler`.

---

## 🤖 Models Used
- **Random Forest**: Out-of-Bag score ≈ 0.7356
- **XGBoost Classifier**: Accuracy ≈ 75%
- **Support Vector Machine (SVM)**: Used with RBF kernel and class balancing

---

## 📈 Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score
- Classification report evaluated both on training and test split
- Random Forest and XGBoost showed strong balance between bias and variance

---

## 📤 Output
- Final predictions exported to `second_competition_v2.csv`
- Columns: `PassengerID`, `Transported`

---

## 🚀 Future Improvements
- Incorporate feature selection methods (e.g., SHAP or Recursive Feature Elimination)
- Use ensemble stacking of SVM, RF, and XGBoost
- Optimize hyperparameters with `GridSearchCV` across all models