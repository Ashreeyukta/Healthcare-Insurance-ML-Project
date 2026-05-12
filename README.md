# Predicting Healthcare Insurance Costs and Risk Categories Using Machine Learning

## Project Overview
This project uses machine learning to predict healthcare insurance costs and classify individuals into healthcare risk categories. The analysis includes data preprocessing, exploratory data analysis, feature engineering, PCA dimensionality reduction, regression modeling, classification modeling, and ensemble model comparison.

## Dataset
The dataset contains 1,338 insured individuals with demographic, lifestyle, clinical, financial, and risk-related variables.

Main features include:
- Age
- Sex
- BMI
- Children
- Smoker status
- Region
- Blood pressure
- Exercise frequency
- Pre-existing condition
- Occupation risk
- Annual income
- Insurance charges

After cleaning missing values, the final dataset contains 1,335 observations.

## Project Workflow
1. Load and inspect dataset
2. Remove missing values
3. Perform exploratory data analysis
4. Apply log transformation to insurance charges
5. Create engineered features:
   - smoker_binary
   - bmi_smoker_interaction
   - age_bp_risk
6. Create risk categories:
   - Low
   - Medium
   - High
7. Apply preprocessing:
   - numerical scaling
   - categorical one-hot encoding
8. Train regression models
9. Train classification models
10. Compare ensemble models
11. Evaluate model performance

## Models Used

### Regression Models
- Linear Regression
- Ridge Regression
- Lasso Regression
- Support Vector Regression (SVR)
- Random Forest Regressor
- XGBoost Regressor

### Classification Models
- Logistic Regression
- Support Vector Machine (SVM)
- Multi-Layer Perceptron (MLP) Neural Network
- Random Forest Classifier
- XGBoost Classifier

## Evaluation Metrics

### Regression
- MAE
- RMSE
- R² Score
- Cross-validation R²

### Classification
- Accuracy
- Macro F1-score
- AUC-ROC
- Confusion Matrix

## Key Results
- XGBoost achieved the best regression performance with an R² score of approximately 0.889.
- Random Forest and XGBoost achieved the highest classification accuracy of approximately 92%.
- SVR performed best among the traditional/non-ensemble regression models.
- SVM performed best among the core classification models.
- Feature engineering improved the model’s ability to capture smoking-related and age-related health risk patterns.

## Files in This Repository
├── README.md
├── Final_Report_Shreeyukta_Aryal.pdf
├── Project_Presentation_Shreeyukta_Aryal.pptx
├── health_insurance_cost_and_risk_dataset.csv
├── healthcare_insurance_ml_project.ipynb
├── requirements.txt

## Installation and Setup

### 1. Clone the Repository

```
git clone https://github.com/Ashreeyukta/Healthcare-Insurance-ML-Project.git

### 2. Open the Project Folder

```
cd Healthcare-Insurance-ML-Project
```

### 3. Install Required Libraries

```
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```
jupyter notebook
```

### 5. Open the Notebook File

Open:

```
health_insurance_cost_Shreeyukta_Aryal.ipynb
```

and run all cells from top to bottom.

---

## Required Libraries

The project uses the following Python libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- scipy
- xgboost
- tabulate
- jupyter



