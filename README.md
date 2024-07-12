# Sentiment_Analysis
A Sentiment Analysis project using VADER (Valence Aware Dictionary and sEntiment Reasoner) approach utilizing the SentimentIntensityAnalyzer model of NLTK, and comparing its results with RoBERTa model by huggingface. The dataset used is that of a bunch of Amazon Reviews.

The model used here for VADER approach does not yield accurate results. SentimentIntensityAnalyzer has a predefined sets of scores for various words of English. It assigns these scores to the words in the given sentence by tokenizing them, and removing any stop words. The main problem with this approach is, the model does not take in to account the connection between words or the different ways a word might be used in different sentences. The VADER approach uses a bag of words here.

The RoBERTa (Robustly optimized BERT approach) model on the other hand, is based on the Transformer architecture, particularly the encoder part. It leverages attention mechanism to learn contextual relationship between words in a sentence. The Transformer Encoder using a Self-Attention mechanism to compute the representation of tokens by considering all other tokens in the sentence. A number of Feedforward Neural Networks process the outputs from the self-attention mechanism. 

Overall the results from the two models in terms of negative or positive labelling of a review are more or less the same (excluding reviews which have a more meaning behind them), but the degree of the labelling is drastically different. The rating for each review as to the negativity, positivity or the neutrality is drastically more in RoBERTa model as compared to the VADER approach.

The link to the kaggle dataset is given below:
https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews

I could not include it in the repository due it being a very large file (approx. 254 MBs and Github has a limit of 25 MB).

Happy Coding! :)
