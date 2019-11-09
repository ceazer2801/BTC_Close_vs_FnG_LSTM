# LSTM Bitcoin Predictions
## Closing Price vs. Fear and Greed Index

__Which one has better predictability?__


### Daily Close Price
Using the daily close price as both a feature and a target in our RNN with an 'Adam' optimizer, and utilizing mean squared error for our loss funtion we come to a loss of 0.0133 after only 10 epochs.  This is a 10x decrease from the initial loss of 0.1294.  With continued epochs this model would continue to get lower loss results.  


### Fear and Greed Index
Using the fear and greed index as a feature for our target of daily close prices with the same 'Adam' optimizer, utilizing the same mean squared error we only come down to a loss result of 0.0457 after the same 10 epochs.  This is 4x higher than the results from the close price model.  This model also never reacted to the sharp increase in price that occured in our dataset.

### Closing
In review the Daily close price is a much more powerful descriptor of the target than the fear and greed index.