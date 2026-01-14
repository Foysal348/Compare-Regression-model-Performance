# Compare-Regression-model-Performance
**1. Overview of Evaluation Metrics**

Mean Squared Error (MSE):
Measures the average squared difference between predicted and actual values. Lower values indicate better performance.

Mean Absolute Error (MAE):
Measures the average absolute prediction error. Lower values mean predictions are closer to true values.

R² Score (Coefficient of Determination):
Indicates how well the model explains the variance in the target variable. Values closer to 1 represent stronger explanatory power.

**2. Model-wise Performance Analysis**

*Linear Regression*

MSE: 0.020269

MAE: 0.111376

R²: 0.9459

Interpretation:
Serves as a strong baseline model but is limited in capturing non-linear relationships, resulting in the weakest overall performance among the models.

*Random Forest Regressor*

MSE: 0.018647

MAE: 0.108201

R²: 0.9502

Interpretation:
Improves upon linear regression by modeling non-linear patterns. However, it underperforms compared to boosting-based and ensemble stacking approaches.

*Gradient Boosting Regressor*

MSE: 0.015155 (lowest)

MAE: 0.098902

R²: 0.9596 (highest)

Interpretation:
This model demonstrates the best overall performance, achieving the lowest error and the highest explanatory power. It effectively balances bias and variance.

*Voting Regressor*

MSE: 0.015919

MAE: 0.100838

R²: 0.9575

Interpretation:
Provides stable and reliable predictions by aggregating multiple models, but it does not outperform the strongest individual learner.

*Stacking Regressor*

MSE: 0.015215

MAE: 0.098687 (lowest MAE)

R²: 0.9594

Interpretation:
Performs nearly as well as Gradient Boosting, with slightly better average absolute error, indicating more consistent predictions.

**Overall Model Ranking**

<img width="851" height="314" alt="image" src="https://github.com/user-attachments/assets/ba3a920d-eb40-471c-8e82-4bf86c1e0160" />
