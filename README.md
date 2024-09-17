XGBoost model using mock random data, once the data is filled in I should juse be able drop it in and do a little tuning and we will be done.
-------------------------------------------------------------------------------
This code splets the data into training, validaiton, and held-out test sets.
The values of the features are scaled using the training data.
The XGBoost model is then trained. A grid search is performed to tune the hyperparameters.
The best model is then trained on the entire training data and the held-out test data is used to evaluate the model.
The confusion matrix, accuracy, precision, recall, f1-score, sensitivity, and negative predictive value are all calculated for the held-out test data.
The feature importances are then plotted for the top features for each type (weight, gain, cover).
