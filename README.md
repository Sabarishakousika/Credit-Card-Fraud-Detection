# Credit-Card-Fraud-Detection
# 💳 Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning techniques. It uses a real-world dataset of anonymized transactions with a strong class imbalance.

---

## 📁 Dataset

Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

- **Rows**: 284,807 transactions
- **Columns**: 30 features (`V1` to `V28`, `Time`, `Amount`) + `Class` label
- `Class`: 0 = Non-Fraud, 1 = Fraud (only ~0.17% fraud)

---

## 🔍 Exploratory Data Analysis (EDA)

- Count plot showing heavy class imbalance
- Percentage of fraudulent transactions
- Correlation heatmap to identify important features for fraud detection

---

## ⚙️ Preprocessing

- Scaled the `Amount` column using `StandardScaler`
- Dropped or skipped `Time` column if missing
- Rearranged columns so `Class` is at the end

---

## 🤖 Model Used

### ✅ Logistic Regression
- Simple, interpretable, and effective for baseline fraud detection
- Trained on 80% of the data, evaluated on 20%

---

## 📈 Evaluation Metrics

- **Confusion Matrix**
- **Classification Report**: Precision, Recall, F1-score
- **ROC Curve** with **AUC Score**

Example ROC AUC Score:
```
ROC AUC Score: ~0.98
```

---

## ✅ Results

| Metric            | Value (Example) |
|-------------------|-----------------|
| Accuracy          | High (but not useful alone) |
| Precision (Fraud) | High            |
| Recall (Fraud)    | Critical        |
| AUC Score         | ~0.98           |

---

## 💡 Conclusion

- Logistic Regression performs well on the imbalanced dataset.
- ROC AUC and Recall are more important than plain accuracy in fraud detection.
- Project successfully shows how to detect fraud with interpretable ML.

---

## 🚀 Future Improvements

- Apply SMOTE or undersampling
- Try ensemble models like Random Forest or XGBoost
- Use cross-validation and hyperparameter tuning

---

## 👨‍💻 Author

**Sabarisha**  
Internship Project – Credit Card Fraud Detection  
