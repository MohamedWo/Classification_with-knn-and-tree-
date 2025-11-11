# PredictSmart - Mobile Price Classification

**PredictSmart** is a smart project that predicts the **price range of mobile phones** using Machine Learning.  
It classifies phones into 4 categories: **Low, Medium, High, Very High** based on their features.

---

## **Dataset**
- Kaggle: [Mobile Price Classification Dataset](https://www.kaggle.com/code/usmohamed/pricesmart))
- Features include:
  - battery_power, ram, int_memory, px_height, px_width, mobile_wt, sc_h, sc_w, etc.
- Target: `price_range` (0: Low, 1: Medium, 2: High, 3: Very High)

---

## **Features**
- Multi-class classification
- Models used:
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors (KNN)
- Data preprocessing:
  - Missing value handling
  - Label encoding for categorical features
  - Feature scaling (StandardScaler)

---

## **Usage**
1. Prepare dataset (`train.csv`, `test.csv`)  
2. Preprocess the data (handle categorical, scale numeric features)  
3. Train a model:

```python
# Example: Logistic Regression
logreg.fit(X_train_scaled, y_train)
y_pred = logreg.predict(X_test_scaled)
# Classification_with-knn-and-tree-
