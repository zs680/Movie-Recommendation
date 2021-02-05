# Movie-Recommendation
The datasets have been collected from 
https://www.kaggle.com/rounakbanik/the-movies-dataset.

In this project we build a collaborative, content-based and a hybrid recommender system. We also train a probabilistic model to predict average rating.

In Regression.ipynb we clean movies_metadata and credits datasets of 45k movies. We train various regression models and tune hyperparameters through GridSearch.  As a result we find a Stacking model on a local machine with MSE 0.39 

In Collaborative_recommender.ipynb we build a collaborative filtering for rating dataset of 26 million ratings of 270k users considering only users with number of ratings in above 5 percent. We train both a model base (SVD) and a memory base (KNNwihMeans)  recommender and tuned hyperparameters for them through GridSearch. We  obtain a recommender model with .87 accuracy.

In Content_Based_Recommender.ipynb we use movie reviews of 45k movies in movies_metadata and train a word2vec embedding. We extract TF-IDF weighted average of word vectors and build a content based recommender based on cosine similarity matrix of movies' reviews TF-IDF weighted averages. We also build a hybrid recommender by combining the above collaborative and content-based recommender. 


