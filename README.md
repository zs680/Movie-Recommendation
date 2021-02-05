# Movie-Recommendation
The datasets have been collected from 
https://www.kaggle.com/rounakbanik/the-movies-dataset

In this project we build a collaborative, content-based and a hybrid recommender system. We also train a probabilistic model to predict average rating.

In Regression.ipynb we clean metadata and credit datasets of 45k movies. We  train We tuned hyperparameters through GridSearch for various regressors.  Built a Stacking model on a local machine with MSE 0.39 
Built a collaborative filtering for rating dataset of 26 million ratings of 270k users considering only users with number of ratings in above 5 percent. Tuned hyperparameters for both SVD and KNNwihMeans models through GridSearch to obtain a recommender model with .87 accuracy
Built a content-based recommender using movie reviews of 45k movies in metadata dataset by training a word2vec embedding and extracting TF-IDF weighted average of word vectors
Built a hybrid recommender by combining the above collaborative and content-based recommender
