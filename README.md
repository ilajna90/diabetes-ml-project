# DIABETES PREDICTION USING MACHINE LEARNING

## Project Overview

This project aims to predict whether a patient has diabetes based on clinical and diagnostic features using machine learning models. It demonstrates a complete ML pipeline from data preprocessing to model evaluation, with a focus on healthcare relevance.

---

## Objective

To build a predictive model that can classify patients as diabetic or non-diabetic using features such as glucose level, BMI, insulin, and age.

---

## Dataset

* **Name**:Pima Indians Diabetes Dataset
* **Source:** Kaggle
* **Description:** Contains medical diagnostic measurements for predicting diabetes

### Features:

* Pregnancies
* Glucose
* Blood Pressure
* Skin Thickness
* Insulin
* BMI
* Diabetes Pedigree Function
* Age

### Target:

* **Outcome**

  * 0 → Non-diabetic
  * 1 → Diabetic

---

## Project Workflow

### 1. Data Loading

* Loaded dataset from CSV using pandas

### 2. Data Understanding

* Used `df.info()` and `df.describe()` to analyze structure and statistics

### 3. Data Cleaning

* Identified biologically invalid zero values in features like Glucose and BMI
* Treated them as missing values
* Replaced missing values using **median imputation** (robust to outliers)

### 4. Exploratory Data Analysis

* Visualized class distribution
* Used correlation heatmap to identify relationships between variables

### 5. Feature Selection

* Separated input features (X) and target variable (y)

### 6. Train-Test Split

* Split data into 80% training and 20% testing sets

### 7. Model Building

* Logistic Regression (baseline model)
* Random Forest (ensemble model for improved performance)

### 8. Model Evaluation

* Accuracy
* Precision
* Recall
* F1 Score

---
## Models Used

### Logistic Regression

* Simple and interpretable baseline model

### Random Forest Classifier

* Ensemble model that captures non-linear relationships
* Provided better performance compared to Logistic Regression

---

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | **~77%**     |
| Random Forest       | **~88%** |

---

## Evaluation Metrics

* **Accuracy:** Overall correctness of predictions
* **Precision:** Correctness of positive predictions
* **Recall:** Ability to identify actual diabetic cases
* **F1 Score:** Balance between precision and recall

---

## Key Insights

* **Glucose** is the most important feature influencing predictions
* **BMI and Age** also contribute significantly
* Results align with known clinical understanding of diabetes

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## How to Run the Project

1. Clone the repository
2. Open the notebook (`diabetes_prediction.ipynb`)
3. Run all cells sequentially
4. Ensure `diabetes.csv` is in the same directory

---

## Project Structure

```
diabetes-ml-project/
│── diabetes_prediction.ipynb
│── diabetes.csv
│── README.md
```

---

## Future Improvements

* Hyperparameter tuning
* Cross-validation
* Try advanced models (e.g., XGBoost)
* Use larger and more diverse healthcare datasets

---

## Conclusion

This project demonstrates how machine learning can be applied to healthcare data for disease prediction. It highlights the importance of proper data preprocessing, model selection, and evaluation in building reliable predictive systems.

---

## Author

Anjali Mohan
(Biochemistry + AI/ML Enthusiast)

---
