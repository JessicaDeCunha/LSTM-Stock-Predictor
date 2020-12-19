# LSTM Stock Predictor

![deep-learning.jpg](Images/deep-learning.jpg)

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the [Crypto Fear and Greed Index (FNG)](https://alternative.me/crypto/fear-and-greed-index/) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. You have been asked to help build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.

I used Deep Learning Recurrent Neural Networks to model bitcoin closing prices. One model will use the FNG indicators to predict the closing price while the second model will use a window of closing prices to predict the nth closing price.

- - -

# Prerequisites

- Numpy
- Pandas
- Scikit-learn
- TensorFlow
- Keras

- - -

# Prepared the data for training and testing

For each model, I used 70% of the data for training and 30% of the data for testing.

Applied a MinMaxScaler to scale the data for the model.

Finally, reshaped the data to fit the model's requirement of (samples, time steps, features).

- - - 

# The Architecture of the model

In each Jupyter Notebook, you will see the same custom LSTM RNN architecture. The same parameters and training steps were used for each model. This was necessary to compare each model accurately.

## LSTM Stock Predictor Using Closing Prices

In this notebook the custom LSTM RNN uses a 10 day window of Bitcoin closing prices to predict the 11th day closing price. Model performance is shown below.



- - - 

# Built with
- Python
- Scikit-learn
- TensorFlow
- Keras

- - -

### Resources

[Keras Sequential Model Guide](https://keras.io/getting-started/sequential-model-guide/)

[Illustrated Guide to LSTMs](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)

[Stanford's RNN Cheatsheet](https://stanford.edu/~shervine/teaching/cs-230/cheatsheet-recurrent-neural-networks)

- - -
