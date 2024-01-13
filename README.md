# Sentiment Analysis using MLP, CNN and LSTM in Keras

## In this problem, we are trying to build a classifier to analyze the sentiment of reviews. We have preprocessed the data using the folloowing steps : 

i. You can use binary encoding for the sentiments , i.e y = 1 for positive senti-
ments and y = −1 for negative sentiments.
ii. The data are pretty clean. Remove the punctuation and numbers from the
data.
iii. The name of each text file starts with cv number. Use text files 0-699 in each class for training and 700-999 for testing.
iv. Count the number of unique words in the whole dataset (train + test) and print it out.
v. Calculate the average review length and the standard deviation of review lengths. Report the results.
vi. Plot the histogram of review lengths.
vii. To represent each text (= data point), there are many ways. In NLP/Deep Learning terminology, this task is called tokenization. It is common to rep- resent text using popularity/ rank of words in text. The most common word in the text will be represented as 1, the second most common word will be represented as 2, etc. Tokenize each text document using this method.2
viii. Select a review length L that 70% of the reviews have a length below it. If you feel more adventurous, set the threshold to 90%.
ix. Truncate reviews longer than L words and zero-pad reviews shorter than L so that all texts (= data points) are of length L.

## Now we create Word Embeddings using tokenizer from Keras. It can yield bag of words, one-hot encoded features. 

## We have trained an MLP with 3 hidden layers. 

## Each word is represented to LSTM as a vector of 32 elements and the LSTM is followed by a dense layer of 256 ReLUs. Use a dropout rate of 0.2 for both LSTM and the dense layer. 

## Although CNNs are mainly used for image data, they can also be applied to text data, as text also has adjacency information. We have inserted a Conv1D layer that has 32 feature maps in a CNN. 
