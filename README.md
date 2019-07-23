# DJIA-IBM-Stock-Prediction
Predicting IBM stocks from 2006 to 2018 using recurrent neural networks

Source: https://www.kaggle.com/szrlee/stock-time-series-20050101-to-20171231

I took specifically the csv dataset from IBM to predict IBM stocks

I built 6 LSTM layers for better training and accuracy, given that the dataset has over 3000 rows. However, I chose 10 epochs for training to get a rough accuracy when applying test sets in a short time. What I noticed was that the loss was trending downward to near-zero.

Also, I chose 120 timesteps for each row to train and increase the likelihood of predicting the open stock value of the next date, given the previous dates.

After choosing number of timesteps, LSTM layers, and epochs, we see that the loss is trending downward with each epoch and that the shape of the predicted shape is nearly identical to that of the actual dataset, with a slight shift
