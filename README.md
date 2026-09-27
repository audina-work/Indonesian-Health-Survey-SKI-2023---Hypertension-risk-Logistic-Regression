# Indonesian-Health-Survey-SKI-2023-Hypertension-risk-Logistic-Regression
Hypertension Risk Factors Using Logistic Regression Model in R and Python

## Background
  According to World Health Organization (WHO) projections for 2025, an estimated 1.4 billion adults aged 30–79 worldwide suffer from hypertension. Indonesia faces a notably high prevalence of hypertension, as reflected in the 2023 SKI results: the prevalence among the population aged 15 and older is 8% based on physician diagnosis and 29.2% based on blood pressure measurements.This reveals a significant knowledge gap—exceeding 20%—indicating that the majority of individuals with hypertension in Indonesia are unaware of their condition. This final project employs logistic regression to develop a model explaining the relationship between these sociodemographic factors and hypertension status as determined by measurement.
## Data
- Source: https://www.badankebijakan.kemkes.go.id/hasil-ski-2023/
- Size: 638.178 observations, 7 variables
- Target: hypertension status (binary)
- Note: raw data is not included due to [usage terms].
## Methods
1. Cleaning data
2. Exploratory Data Analysis (EDA)
3. Handling class imbalance with ROSE
4. Multivariate logistic regression
5. Multicollinearity check with VIF
6. Validation with k-fold cross-validation (k = 10)
7. Evaluation: sensitivity, AUC, confusion matrix
## Key Results
- AUC: 0,7131
- Sensitivity: 70.5%
- Significant risk factors: regional characteristics, age, gender, marital status, employment status and Prosperous Family Card Ownership Status 

