# Convolve Hackathon

## Accuracy of the Model : 
0.84307
## Rank : 
101/500 (<a href="https://unstop.com/hackathon/convolve-a-mlai-hackathon-for-the-future-cisco-524330/offline-round/274359">Result</a>) (<a href="https://www.kaggle.com/competitions/convolve-epoch1/data">kaggle site</a>)
## Experience : 
Learnt about the different models that can be used for <b>Log Anomaly Detection</b> we employ the gensim implementation of Word2Vec to encode our logs as fixed length numerical vectors. Logs are noteably not the natural usecase for word2vec, but this appraoch attemps to leverage the fact that logs lines themselves, like words, have a context, so encoding a log based on its co-occurence with other logs does make some intuitive sense.we employ the SOMPY implementation of the Self-Organizing Map to train our model. This function simply makes it a bit easier for the user to interact with the sompy training requirements. This function returns a trained model. If the map successfull converged then it should consist of nodes in our N-dimensional log space that are well ordered and provide an approximation to the topology of the logs in our training set.During training we also, compute the distances of our training data to the trained map as a baseline to build a threashold.

