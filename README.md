# HDFC VWAP Prediction using Stacked LSTM RNN
This project aims to predict the VWAP of HDFC using Stacked LSTM RNN model.
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
The Stacked LSTM RNN model used in this project consists of 2 LSTM layers with 20 units and 10 units each ,

followed by a Dense Output layer with 1 unit

Optimizer= Adam

Loss=mse

Early stopping also utilised
<img width="416" alt="image" src="https://github.com/vaasew/stock_market_price_prediction/assets/79396917/a5f50a00-f0c0-40c5-b403-ed51e0b7ce08">



The input to the model is a sequence of previous 100 days closing stock prices, and the output is the predicted closing stock price for the next day.

# Results
The model was trained for 100 epochs with a batch size of 30, 
(as early stopping utilised training terminated at 32 epochs)


and achieved - 

rmse of 42.006 on test data.


# Prediction Plots

The following graph shows the predicted stock prices over actual prices of HDFC for the train and test data -

![image](https://github.com/vaasew/stock_market_price_prediction/assets/79396917/eee8eeca-7fba-4c0e-9d91-c855b3124c3a)



 Prediction for next 20 days -
 
![image](https://github.com/vaasew/stock_market_price_prediction/assets/79396917/60a50fbe-ea5f-42bf-bc06-5ce7bac3e571)


orange - future predicted data for next 20 days



# Conclusion
The Stacked LSTM RNN model was able to predict the vwa prices of HDFC with a good degree of accuracy, as evidenced by the graphs and acceptable root mean squared error on the test data. However, it should be noted that stock price prediction is a complex and uncertain task, and this model should not be used for making 
investment decisions without further analysis and consultation with a financial advisor.

