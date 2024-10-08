# Regression Analysis on Oil Datasets

## Project Overview
This project involves regression analysis on three different oil datasets:
1. **Maize Oil**
2. **Rapeseed Oil**
3. **Olive Oil**

The objective of the analysis is to identify which machine learning models perform the best in predicting the target variables from these datasets. Several models, including linear and tree-based regressors, were evaluated based on their performance using 5-fold cross-validation mean squared error (MSE) scores.

## Dataset
1. **Maize Oil Dataset**: https://raw.githubusercontent.com/sandroj87/EVOODec/refs/heads/main/evoodec/spectra/mais_seed_oil.csv
2. **Rapeseed Oil Dataset**: https://raw.githubusercontent.com/sandroj87/EVOODec/refs/heads/main/evoodec/spectra/rapeseed_oil.csv
3. **Olive Oil Dataset**: https://raw.githubusercontent.com/sandroj87/EVOODec/refs/heads/main/evoodec/spectra/monocultivar_frantoio.csv

All datasets follow the same structure and were subjected to the same regression analysis.

## Models Used
The following machine learning models were used for regression analysis:
1. **PLS Regression** (Partial Least Squares Regression)
2. **KNeighborsRegressor**
3. **Linear Regression**
4. **Decision Tree Regressor**
5. **Random Forest Regressor**

## Results by Dataset

### 1. **Maize Oil**
The 5-fold cross-validation MSE scores for the maize oil dataset are as follows:

| Model                  | CV MSE               |
|------------------------|----------------------|
| PLS Regression          | 0.1283               |
| KNeighborsRegressor     | 0.0002               |
| Linear Regression       | 0.1283               |
| Decision Tree Regressor | 0.0002               |
| Random Forest Regressor | 0.0001               |

### 2. **Rapeseed Oil**
The 5-fold cross-validation MSE scores for the rapeseed oil dataset are as follows:

| Model                  | CV MSE               |
|------------------------|----------------------|
| PLS Regression          | 0.6886               |
| KNeighborsRegressor     | 0.0021               |
| Linear Regression       | 0.6886               |
| Decision Tree Regressor | 0.0023               |
| Random Forest Regressor | 0.0010               |

### 3. **Olive Oil**
The 5-fold cross-validation MSE scores for the olive oil dataset are as follows:

| Model                  | CV MSE               |
|------------------------|----------------------|
| PLS Regression          | 0.3671               |
| KNeighborsRegressor     | 0.0016               |
| Linear Regression       | 0.3671               |
| Decision Tree Regressor | 0.0011               |
| Random Forest Regressor | 0.0006               |

## Summary of Findings
- **Tree-based models**, particularly the **Random Forest Regressor**, consistently showed the best performance across all datasets, achieving the lowest cross-validation MSE scores.
- **Linear models** such as PLS Regression and Linear Regression tended to perform less effectively compared to tree-based models, especially in datasets like rapeseed and olive oil.
- **KNeighborsRegressor** performed reasonably well but was slightly outperformed by Random Forest in all datasets.

## Conclusion
This analysis highlights that tree-based models, especially the **Random Forest Regressor**, are the most effective for regression tasks in this context. The ability of Random Forest to handle non-linearities and interactions between features likely contributed to its superior performance across the maize oil, rapeseed oil, and olive oil datasets.
