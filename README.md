# Multi-Step Forecasting with LSTM Model

This is a brief summary of the steps to test the LSTM model for multi-step forecasting in unseen multivariate time series data.

## Data Loading
- Load the unseen multivariate time series data (test set) using the appropriate file path.
- Ensure the dataset has similar features as the training set.

## Data Preprocessing
- Apply the same preprocessing steps as in the training phase.
- Drop any unnecessary columns, handle missing values, and scale features using Min-Max scaling.

## Sequence Preparation
- Use the `create_sequences` function to prepare input sequences for the LSTM model.
- Set appropriate values for `n_steps_in` and `n_steps_out`.

## Model Loading
- Load the pre-trained LSTM model using the provided code.

## Predictions
- Use the loaded model to make predictions on the test set (`X_test_predict`).
- Obtain the predicted values (`y_pred`) for each sequence.

## Evaluation
- Evaluate the model's performance using appropriate metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE).
- Compare the predicted values (`y_pred`) with the actual values (`y_test`) to assess accuracy.

## Visualizations
- Optionally, create visualizations such as line plots to compare actual vs. predicted values.
- Visualize the layer structure of the model using the `plot_model` function.
