# deeplearning-homework

## Matthew Newkirk UW FinTech Part-Time Unit 14 HW - Deep Learning

### Summary of Findings

#### Which model has a lower loss?

The model that uses only close to predict close has a better lose at just .002 compared to .10 for the model using sentiment.

#### Which model tracks the actual values better over time?

If we consider this question in terms of plotting Real vs. Predicted values, the model using close to predict close performs better.

#### Which window size works best for the model?
Both models see much better performance in terms of lower model loss value from a smaller window size. For the model using just close a window size of 1 or 2 seemed to work best, though further testing should be conducted to determine whether or not a window size that small may lead to over fitting. For the model using sentiment, the model stayed fairly consistent at a loss of.07 for window size values less than 5, but window sizes less than 5 cause the plot of Real vs. Predicted closing price to reveal a much flatter plot of Predicted values, potentially indicating that sentiment alone is too small a feature set for this LSTM model to adequately learn and predict closing values.
