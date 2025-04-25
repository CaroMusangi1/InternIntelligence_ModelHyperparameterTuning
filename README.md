```
# 🧠 HYPERPARAMETER TUNING — RANDOM FOREST ON IRIS DATASET

## PROJECT OVERVIEW 📌
This project demonstrates how to improve model performance through hyperparameter tuning.  
Using the classic **Iris dataset**, we apply `GridSearchCV` to a **Random Forest Classifier** to find the best parameter combination.

---

## KEY CONCEPTS 🔑

🎛️ Hyperparameter Tuning — Adjusting settings like `n_estimators`, `max_depth`  
🧮 Grid Search — Testing all possible combinations of parameters  
🔄 Cross-Validation — Evaluating model performance across multiple folds

---

## WORKFLOW STEPS ⚙️

### 🌱 LOAD AND PREPROCESS DATA
- Load Iris dataset from `sklearn.datasets`
- Extract features (`X`) and target (`y`)

### ✂️ SPLIT THE DATASET
- Use `train_test_split()` to split into training and test sets (80/20)

### 🔧 DEFINE HYPERPARAMETER GRID
```python
param_grid = {
  'n_estimators': [50, 100, 150],
  'max_depth': [3, 5, 10],
  'min_samples_split': [2, 5, 10]
}
```

### 🧠 TUNE WITH GRIDSEARCHCV
- Use `GridSearchCV` with `RandomForestClassifier`  
- Automatically selects the best parameter combination

### 🏆 EVALUATE THE BEST MODEL
- Print the best parameters  
- Test accuracy on the test set  
- Optional: visualize feature importance or confusion matrix

---

## LIBRARIES USED 🧪

- **scikit-learn** — Modeling, tuning, evaluation  
- **numpy** — Numerical operations  
- **matplotlib** — Visualizations (optional)  
- **pandas** — Data manipulation (optional)

---

## HOW TO USE THIS PROJECT 🚀

1. Open the notebook in **Google Colab**  
2. Run all cells step-by-step  
3. Modify the `param_grid` to test different parameters  
4. (Optional) Save the model using `joblib`

---

## OUTPUT 📦

✅ Best hyperparameters for the model  
✅ Accuracy and evaluation metrics on test set  
✅ (Optional) Feature importance or confusion matrix

---
