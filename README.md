```markdown
# 🧠 HYPERPARAMETER TUNING — RANDOM FOREST ON IRIS DATASET

## <u>PROJECT OVERVIEW</u> 📌
This project demonstrates how to improve model performance through **hyperparameter tuning**.  
We use the classic **Iris dataset** and apply `GridSearchCV` to a **Random Forest Classifier** to find the best parameter combination.

---

## <u>KEY CONCEPTS</u> 🔑
- **HYPERPARAMETER TUNING**: Adjusting settings like `n_estimators`, `max_depth`  
- **GRID SEARCH**: Testing all possible combinations of parameters  
- **CROSS-VALIDATION**: Evaluating model performance across multiple folds

---

## <u>WORKFLOW STEPS</u> ⚙️

### 🌱 <u>LOAD AND PREPROCESS DATA</u>
- Load the Iris dataset from `sklearn.datasets`  
- Extract features (`X`) and target (`y`)

### ✂️ <u>SPLIT THE DATASET</u>
- Split data into training and test sets using `train_test_split()` (80/20)

### 🔧 <u>DEFINE HYPERPARAMETER GRID</u>
```python
param_grid = {
  'n_estimators': [50, 100, 150],
  'max_depth': [3, 5, 10],
  'min_samples_split': [2, 5, 10]
}
```

### 🧠 <u>TUNE WITH GRIDSEARCHCV</u>
- Use `GridSearchCV` with **RandomForestClassifier** to find the best parameter combination

### 🏆 <u>EVALUATE THE BEST MODEL</u>
- Print the best parameters  
- Test accuracy on the test set  
- (Optional) Visualize feature importance or confusion matrix

---

## <u>LIBRARIES USED</u> 🧪
- **SCIKIT-LEARN** — Modeling, tuning, and evaluation  
- **NUMPY** — Numerical operations  
- **MATPLOTLIB** — Visualizations (optional)  
- **PANDAS** — Data manipulation (optional)

---

## <u>HOW TO USE THIS PROJECT</u> 🚀
1. Open the notebook in **Google Colab**  
2. Run all cells step-by-step  
3. Modify the `param_grid` to test different parameters  
4. (Optional) Save the model using `joblib`

---

## <u>OUTPUT</u> 📦
- Best hyperparameters for the model  
- Accuracy and evaluation metrics on the test set  
- (Optional) Feature importance or confusion matrix

---

---
