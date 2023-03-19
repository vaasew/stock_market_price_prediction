# HDFC Stock Price Prediction using Stacked LSTM RNN
This project aims to predict the stock prices of HDFC using Stacked LSTM RNN + ANN model.
# Dataset
The dataset used in this project is obtained from Kaggle - https://www.kaggle.com/datasets/rohanrao/nifty50-stock-market-data. It consists of the historical stock prices of HDFC from 2000 to April 2021.
# Dependencies
The following libraries are required to run this project:

    Pandas
    Numpy
    Matplotlib
    Scikit-Learn
    Keras
# Model Architecture
The Stacked LSTM RNN +ANN model used in this project consists of 3 LSTM layers with 50 units each with one 0.2 dropout layer after the first LSTM, 
followed by a Dense layer with 25 units with relu activation and 
then a Dense layer with 1 unit.

The input to the model is a sequence of previous 100 days closing stock prices, and the output is the predicted closing stock price for the next day.

# Results
The model was trained for 100 epochs with a batch size of 60, 


and achieved - 

a root mean squared error of 0.0204 on the scaled train data and 0.0162 on scaled test data.


rmse of 59.24 on scale inversed train data and 47.09 on scale inversed test data.


# Prediction Plots

The following graph shows the predicted stock prices over actual prices of HDFC for the train and test data -

![image](https://user-images.githubusercontent.com/79396917/226197151-3548d340-d76d-467c-bdde-8b940263998f.png)


 Prediction for next 50 days -
 
![image](https://user-images.githubusercontent.com/79396917/226197164-5f67000a-c7c0-49f8-8d59-895ccc3e1963.png)

orange - future predicted data for next 50 days



# Conclusion
The Stacked LSTM RNN model was able to predict the stock prices of HDFC with a good degree of accuracy, as evidenced by the graphs and low root mean squared error on the test data. However, it should be noted that stock price prediction is a complex and uncertain task, and this model should not be used for making 
investment decisions without further analysis and consultation with a financial advisor.

