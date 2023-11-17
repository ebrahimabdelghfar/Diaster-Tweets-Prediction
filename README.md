# Disaster Tweets NLP
This project uses Natural Language Processing (NLP) to classify tweets as talking about a real disaster or not.

## Data
The data comes from the Kaggle competition Real or Not? NLP with Disaster Tweets. It contains a training set train.csv with the tweet text and a target label of 1 for real disaster tweets and 0 for non-disaster tweets. There is also a test set test.csv with just the tweet text that needs to be classified.

## Notebook Overview
The Jupyter notebook TweetsDiaster.ipynb goes through the following steps:

- Imports libraries like NLTK, Pandas, Sklearn
- Loads and explores the train and test CSV data
- Cleans the text by:
  - Converting to lower case
  - Removing punctuation
  - Removing stopwords
  - Stemming words
- Vectorizes the text using CountVectorizer
- Splits data into training and validation sets
- Trains and tunes SVM, Decision Tree, and Gradient Boosting models using GridSearchCV
- Outputs model evaluation metrics like accuracy, precision, recall, F1 score
- Makes sample predictions on new tweets

## Results
The Gradient Boosting model performed the best with ~78% accuracy on the validation set. For the actual Kaggle competition test set it achieved a score of 0.78411.
