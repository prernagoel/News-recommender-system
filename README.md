# News-recommender-system

We use machine learning to build a personalized news articles recommendation system
based on the user’s previous article ratings. Different people have different topics of interest,
and this is not reflected in a single score. Our recommender system helps users instantly
discover news articles to their liking, regardless of how distinct their tastes may be. If a new
user lands on the website/app, we recommend news articles from diverse topics so that the probability
of the user to find the article of his/her interest increases.

Current recommender systems generally fall into two categories: content-based filtering and
collaborative filtering. We experiment with both approaches in our project. For content-based
filtering, we use the TF-IDF (term frequency/inverse-document-frequency) technique for
vectorization of data and further calculate the similarity between articles. We have also used a
topic modeling based approach for the same. For collaborative filtering, the input to our
algorithm is the observed users’ article rating, and we use K-nearest neighbors and matrix
factorization to predict user’s article ratings​ .
