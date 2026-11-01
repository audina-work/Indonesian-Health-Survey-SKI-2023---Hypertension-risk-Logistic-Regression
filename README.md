# Indonesian-Health-Survey-SKI-2023-Hypertension-risk-Logistic-Regression
Hypertension Risk Factors Using Logistic Regression Model in R and Python

## Background
  According to World Health Organization (WHO) projections for 2025, an estimated 1.4 billion adults aged 30–79 worldwide suffer from hypertension. Indonesia faces a notably high prevalence of hypertension, as reflected in the 2023 SKI results: the prevalence among the population aged 15 and older is 8% based on physician diagnosis and 29.2% based on blood pressure measurements.This reveals a significant knowledge gap—exceeding 20%—indicating that the majority of individuals with hypertension in Indonesia are unaware of their condition. This final project employs logistic regression to develop a model explaining the relationship between these sociodemographic factors and hypertension status as determined by measurement.
## Data
- Source: https://www.badankebijakan.kemkes.go.id/hasil-ski-2023/
- Size: 638.178 observations, 7 variables
- Target: hypertension status (binary)
- Note: raw data is not included due to [usage terms].
  
## Methodology
The analytical workflow consists of the following steps:

### 1. Data Cleaning and Preparation
- Inspect the dataset structure, variable types, and data consistency.
- Identify and handle missing values and duplicate observations.
- Recode categorical variables and define the binary hypertension outcome.
- Prepare predictor variables for statistical modeling.

### 2. Exploratory Data Analysis (EDA)
- Examine the distribution of demographic and clinical characteristics.
- Explore the prevalence of hypertension across relevant subgroups.
- Investigate preliminary associations between predictor variables and hypertension.

### 3. Multicollinearity Assessment
- Assess multicollinearity among predictor variables using the Variance Inflation Factor (VIF).
- Identify highly correlated predictors that may affect the stability and interpretability of the regression coefficients.

### 4. Handling Class Imbalance
- Apply Random Over-Sampling Examples (ROSE) to address class imbalance in the training data.
- Preserve the original class distribution in the validation data to obtain an unbiased estimate of model performance.

### 5. Multivariate Logistic Regression
- Develop a multivariate logistic regression model to investigate factors associated with hypertension.
- Estimate regression coefficients, odds ratios, and their corresponding confidence intervals.
- Assess the statistical significance of the predictor variables.

### 6. Model Validation
- Evaluate model performance using 10-fold cross-validation.
- Apply data preprocessing and class balancing within each training fold to prevent data leakage.

### 7. Model Evaluation
Evaluate model performance using the following metrics:
- Sensitivity (Recall)
- Area Under the Receiver Operating Characteristic Curve (ROC-AUC)
- Confusion Matrix

The evaluation focuses on the model's ability to identify individuals with hypertension while assessing its overall discriminatory performance.
**Implementation:** R and Python.

## Key 
- The model achieved a ROC-AUC of 0,7131.
- The model achieved a sensitivity of 70.5%.
- Significant risk factors: Regional characteristics, Age, Gender, Marital status, Employment status and Prosperous Family Card Ownership Status

## Limitations
- The analysis uses cross-sectional survey data.
- The findings represent associations rather than causal relationships.
- Model performance may depend on the selected predictors,
  class balancing strategy, and classification threshold.

