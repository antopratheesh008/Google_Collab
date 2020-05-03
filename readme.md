Sentiment Analysis using LSTM

Sentiment analysis using a LSTM is built using Pytorch framework. Movie review data is used for the classification. 

Brief of the network created:

First, we'll pass in words to an embedding layer. We need an embedding layer because we have tens of thousands of words, so we'll need a more efficient representation for our input data than one-hot encoded vectors.The embedding layer is used for dimensionality reduction, rather than for learning semantic representations.
After input words are passed to an embedding layer, the new embeddings will be passed to LSTM cells. The LSTM cells will add recurrent connections to the network and give us the ability to include information about the sequence of words in the movie review data. 
Finally, the LSTM outputs will go to a sigmoid output layer. We're using a sigmoid function because positive and negative = 1 and 0, respectively, and a sigmoid will output predicted, sentiment values between 0-1.
