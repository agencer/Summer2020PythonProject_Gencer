# Summer2020PythonProject_Gencer
Including codes and data for the Summer 2020 Python Project. 

The name of Project is <i><b>Wag the Dog’ Media</b>: Does the President Distract the Public When Issuing Executive Orders?"</i>

Files Included:

## datascraping_sentimentanalysis_Python_gencer\gencer_ExecutiveOrderScraping.py
- Scrapes all presidential orders from https://www.presidency.ucsb.edu by 
  - its content, 
  - issue no, 
  - issue date, and 
  - url since the presidentcy of Donald Trump.

## datascraping_sentimentanalysis_Python_gencer\gencer_exeorder.csv
- Created by \gencer_ExecutiveOrderScraping.py after scraping.

## datascraping_sentimentanalysis_Python_gencer\gencer_TrumpTweets.csv
- Downloaded from http://www.trumptwitterarchive.com/
- Over 24 thousand Trump tweets, each tweet includes
  - content
  - number of likes
  - numbe of retweets
  
## datascraping_sentimentanalysis_Python_gencer\preprocessing_exeorder.py
- Preprocesses executive orders.
- Creates the beginning and end dates of 1,3,5,7,11, and 15 days intervals around the executive orders
- Applies these intervals to \gencer_TrumpTweets.csv

## datascraping_sentimentanalysis_Python_gencer\gencer_TrumpTweets_2.csv
- Processed version by \preprocessing_exeorder.py that includes
  - Intervals and Search Term results.

## datascraping_sentimentanalysis_Python_gencer\sentiment_analysis_for_tweets.py
- Downloads nltk Twitter corpus data to train a logistic function for sentiment analysis (5000positive \ 5000negative)
- Trains a logistic regression based on the training data (the code from Coursera course: Natural Language Processing).
- Preprocesses each Trump tweet by
  - removing stop words, 
  - removing punctuations,
  - stemming and tokenizing (the code from Coursera course: Natural Language Processing).
- Predicts the sentiment scores of each tweet

## datascraping_sentimentanalysis_Python_gencer\gencer_TrumpTweets_3.csv
- Processed version by \sentiment_analysis_for_tweets.py that includes
  - Sentiment Score of each Tweet

## dataanalysis_R_gencer\dataanalysis_gencer.Rmd
- Runs the linear regressions
- Creates figures with estimates and confidence intervals

## presentation_Latex_gencer\Python_Project.pdf
- Presentation of the Python project

## presentation_Latex_gencer\Graphs
- Includes all figures created by \dataanalysis_gencer.Rmd for the project.
- all in .jpg format.
