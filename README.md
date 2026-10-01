# Time-series-forecasting-for-Amazon-Stock-Price-using-Neural-Networks-and-Random-Forest-models
Time Series Forecasting between Neural Networks and Random Forest

## Model Comparison: Random Forest vs. CNN

Based on the evaluation metrics on the test set:

**Random Forest Regressor:**

Mean Squared Error (MSE): 3912.97

R-squared (R2): -1.75

**Convolutional Neural Network (CNN):**

Mean Squared Error (MSE): 35.66

R-squared (R2): 0.97

## Analysis:

A lower MSE and a higher R2 (closer to 1) indicate better model performance.
The CNN model has a significantly lower MSE (35.66 vs 3912.97) and a much higher R2 (0.97 vs -1.75) compared to the Random Forest model.
The negative R2 for the Random Forest suggests that it performs worse than simply predicting the average closing price of the test set.

The price that CNN predicted, 221.99, is highly similar to the real Amazon closing price on 10/24/2025, 224.21. The price predicted by Random Forest, 107.45, is much lower than the real closing price.

## Conclusion:

Based on these results, the CNN model performed significantly better than the Random Forest model at predicting the Amazon stock closing price on this test set. This is also visually apparent when comparing the individual prediction plots, where the CNN predictions track the actual prices much more closely.

## Reason for CNN's better performance:

The CNN model is better suited for this time-series data because it can effectively learn and capture sequential patterns and dependencies in the stock prices over time. . While Random Forest can capture non-linear relationships, they don't inherently model sequential dependencies or patterns over time as effectively as models designed for sequences.

Thus, the CNN model significantly outperformed the Random Forest model in predicting Amazon stock prices by effectively learning from the sequential nature of the data, a capability less pronounced in models that treat data points independently.
