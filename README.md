# News recommender system

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

Dataset and Attributes

News articles dataset ​ - We created a corpus of ~10,000 news articles taken from multiple
sources, the major contributors being the following: Scroll, HistoryNewsNetwork, The Verge,
and ESPN. The data corpus contains multiple features of the scraped articles including their
date of publication, article id, author name, article headline, article topic.

User Clickstream dataset - ​ Once the user starts consuming news stories, (s)he leaves behind a
clickstream which can be then used to uncover user interests and provide personalized
recommendations. We generated a user clickstream data which contains the following
attributes:

User ID     -  ID given to each unique user on the app

Session ID  -  Refers to each new visit of the user on the app

Article ID  -  A unique ID given to each article

Click       -  Takes the value ‘Yes’ if the article has been clicked by the user, otherwise no.

Time spent  -  Time spent by the user on a particular article in seconds

Rating      -  Rating of an article ranging from 1 to 5. Correlated with time spent.
