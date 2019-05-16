# crude-oil-price-Time-series-forecasting-using-LSTM

This project is based on timeseries forecasting with lstm on price of crude oil 
i.e we will take the existing prices of crude oil and create a lstm(long-short term memory) deep neural network and train it on existing data and see how it is predicting 

Data Source
the data was obtained from 
U.S. Energy Information Administration, Crude Oil Prices: Brent - Europe [DCOILBRENTEU], retrieved from FRED, Federal Reserve Bank of St. Louis;
URL: https://fred.stlouisfed.org/series/DCOILBRENTEU
get the data file in csv format from the above url

LSTM Model:
for this purpose i have used a lstm with 4 layers
Layer (type)                 Output Shape              Param #   
=================================================================
input_1 (InputLayer)         (64, 30, 1)               0         
_________________________________________________________________
lstm_1 (LSTM)                (64, 30, 10)              480       
_________________________________________________________________
lstm_2 (LSTM)                (64, 30, 10)              840       
_________________________________________________________________
dense_1 (Dense)              (64, 30, 1)               11        
=================================================================
Total params: 1,331
Trainable params: 1,331
Non-trainable params: 0

LOSS  FUNCTION: MAE
