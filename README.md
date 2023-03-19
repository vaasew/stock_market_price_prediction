# HDFC Stock Price Prediction using Stacked LSTM RNN
This project aims to predict the stock prices of HDFC using Stacked LSTM RNN model.
# Dataset
The dataset used in this project is obtained from Yahoo Finance. It consists of the historical stock prices of HDFC from January 2010 to April 2021.
# Dependencies
The following libraries are required to run this project:

    Pandas
    Numpy
    Matplotlib
    Scikit-Learn
    Keras
# Model Architecture
The Stacked LSTM RNN model used in this project consists of 3 LSTM layers with 128 units each, followed by a Dense layer with 1 unit.
The input to the model is a sequence of 50 stock prices, and the output is the predicted stock price for the next day.
# Results
The model was trained for 100 epochs, and achieved a mean squared error of 0.0016 on the test data. 
The following graph shows the actual and predicted stock prices of HDFC for the train and test data.
*image*
# Conclusion
The Stacked LSTM RNN model was able to predict the stock prices of HDFC with a high degree of accuracy, as evidenced by the low mean squared error on the test data. However, it should be noted that stock price prediction is a complex and uncertain task, and this model should not be used for making 
investment decisions without further analysis and consultation with a financial advisor.

