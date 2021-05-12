# Movie Review Analysis
1. This analysis is the answer to one question which is 
"Which thing in movie people’s attention drawn most towards it in any movie?" as “More Insights on Reviews”.
2. Easiest Model built with high accuracy for sentiment analysis for reviews by logistic regression.

# Purpose of this analysis
Demonsstraight how to get most out of minimum resource and minimal efforts, in this case, getting started datasets rather than just being expert in data skills by technical parts.

# Dataset
Stanford IMDB Dataset was used in this project which was originally published by researchers of Stanford University. 
In this dataset there are thousands of movie reviews were collected as in 30 reviews per movie, 50-50% positive-negative to get insight.
Original Link: http://ai.stanford.edu/~amaas/data/sentiment/

# Preprocessing
## Part 1: Kaggle dataset with rating and sentiment columns 
It is a major part of which the whole dataset converted in CSV formate with columns Review, Rating, Sentiment by file handling and this preprocessed dataset I am putting on Kaggle and in this project I am using that dataset.
Link:
https://www.kaggle.com/nisargchodavadiya/imdb-movie-reviews-with-ratings-50k
Which is looking like this:
![Data Frame Snap Shot](https://user-images.githubusercontent.com/75474944/117930709-f45a9c80-b31b-11eb-8aa1-bafeb59a6d97.PNG)

## Part 2: Preprocess the text to analyze (Text Clean)
For sentiment analysis text in the whole dataset cleaned by removing punctuation and stop words.
## Part 3: Process text for algorithm for sentiment analysis
Applied STEM on the cleaned text and then converted TF-IDF vectors.

# Model
A very simple Logistic Regression algorithm applied to get higher accuracy more than given in TensorFlow website with RNN with LSTM https://www.tensorflow.org/tutorials/text/text_classification_rnn#stack_two_or_more_lstm_layers

Accuracy of Logistic Regression model without tuning 88% on test data. 
![CM for IMDB Case Study](https://user-images.githubusercontent.com/75474944/117927560-fe7a9c00-b317-11eb-99bb-a8b0ece54aa7.png)

# More Insights on Reviews
Word Cloud on positive and negative reviews can answer a superficially to question that is “Which thing in movie people’s attention drawn most towards it in any movie?”

## Preprocessing for Word Cloud
That is the most sensitive step which only can give superficial insight on this question.
Remove stopwords and punctuations, HTML tags, and combine all positive reviews. Then followed same for negative reviews.
Feed this to word cloud and the next preprocess to insight can only be done directly at word cloud.
 
# Word Cloud
In this word cloud, notice the biggest word if it is a common word which is not leading to insight to question then add that word in stop words for word cloud and plot word cloud again up to when the first word which can derive insight from the word cloud.

Positive Reviews Word Cloud:
![Positive reviews](https://user-images.githubusercontent.com/75474944/117929690-b90b9e00-b31a-11eb-9cd5-b262cdd442ee.png)

Negative Reviews Word Cloud:
![Negative reviews](https://user-images.githubusercontent.com/75474944/117929702-bc068e80-b31a-11eb-84df-42cb8c7782d7.png)

# Conclusion
Answer to Question:
1. People look at the character, story in the movie at first glance.
2. Then they looked at the scene.
3. Many times the story, scene makes the movie bad when the movie gets low ratings.
Note: This dataset was published in 2011 so today’s reviews may make a difference in the answer to this question.

# Acknowledgement
Special thanks or Special acknowledgment goes to Questioner "[Mahesh Bhuva](https://github.com/mahesh1996)".
Publishers (Authors) of  Original this Dataset.
