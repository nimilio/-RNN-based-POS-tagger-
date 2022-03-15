# RNN-based-POS-tagger
Evaluating and extending an RNN based POS tagger with Pytorch

Pipeline for POS tagging using LSTMs and mini-batch training.  
Model evaluation on a number of sources in different languages.  
The neural model represents the data's tokens as non-pretrained embedding vectors. The sequences of embedding vectors are passed through an LSTM layer. The outputs from the recurrent layer are then transformed to probabilities over POS tags by passing them through a fully connected layer and a softmax. 

The task is to predict, for an unseen review, whether it is positive or negative. This is a binary classification task.

Apart from English, Bulgarian, Afrikan and Turkish models are trained and evaluated. Evaluation is compared per RNN model type (LSTM or GRU), one direction or bi-directional, with and without dropout effect and different dimensionalities.

I provide comments after the multiple evaluations of each corpus and final comparisons at the end of the notebook.
