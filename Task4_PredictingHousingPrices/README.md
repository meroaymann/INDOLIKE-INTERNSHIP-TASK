Task 4 - Predicting Housing Prices 

- Overview
This project predicts median housing prices in Boston using classic regression models.  
It explores how features like location, number of rooms, pollution, and property tax impact housing prices.

- Data
- Dataset: Boston Housing Dataset (`housing.csv`)
- Shape: 506 rows × 14 columns
- Target: `MEDV` — Median value of owner-occupied homes in $1000s.

- Methods
- Data preprocessing (cleaning, renaming columns, train/test split)
- Feature scaling with `StandardScaler`
- Model training with:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Random Forest Regressor
- Model comparison using RMSE, MAE, and R² metrics.

- Results
| Model | RMSE | MAE | R² |
| Random Forest | 2.92 | 2.04 | 0.88 |
| Linear Regression | 4.93 | 3.19 | 0.67 |
| Ridge Regression | 4.93 | 3.19 | 0.67 |
| Lasso Regression | 4.97 | 3.19 | 0.66 |

- The Random Forest model achieved the best performance, explaining **88% of price variation**.
- Residuals were normally distributed and unbiased.
- Visualization confirmed strong prediction alignment between actual and predicted prices.

- Key Insight
Housing prices increase with the number of rooms (`RM`) and decrease with poverty levels (`LSTAT`).  
Non-linear models capture complex housing patterns more effectively than simple linear ones.
