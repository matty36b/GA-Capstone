# GA-Capstone

## By Matt Bildzok


For this Capstone, I will be looking into Elon Musk's tweets from 2015 to 2020, and trying to predict if what he tweets will become a highly trafficed and highly engaged tweet, based on what he tweets.


I have gathered the data from the Kaggle linked below:
https://www.kaggle.com/vidyapb/elon-musk-tweets-2015-to-2020/tasks?taskId=1371


I took a look at the data, and cleaned it how I needed it, removing columns that were irrelevant, and focused on what could be the strongest predictors for the target values and variables I was looking for.


I built multiple dataframes from which I built different models, from LassoCV, to Numtinomial Naive Bayes, to Logistic Regression.


I found that the LassoCV models were long winded to run, and didn't provide a strong model, so I had to move on to greener pastures.  To do so, I created another dataframe, Count Vectorized the tweets from Elon Musk, and created new columns to indicate whether the tweets were successful in regards to retweets, replies and likes.


With a base accuracy of 85.5% forpredicting the majority, I had some serious work to do to get a stronger model.


The Multinomial Naive Bayes gave me an accuracy of 86.6%, a small increase if predictability, but an increase nonetheless.  I wanted to create a stronger model, however.

This is where the Sentiment Analysis comes in, I created new columns that showed how negative, neutral and positive each tweet is, with a fourth new column showing the compound score of the three.


After running the new dataframe containing the Count Vectorized tweets and the Sentiment Analysis, I ran it through a gridsearch to find the best parameters.  This ultimately gave me a new model that had 87.4% accuracy, still not a big increase, but an increase from the previous model.

If I had had more time, I would have run more models to try to boost that even more, as well as include my original plan to try to predict any positive or negative changes in any stock market prices.


In the end, I found a model that Elon could use to find a way to tweet things that would increase his interaction and get more of his ideas and philosophies out, as well as be heard even more than he already is.