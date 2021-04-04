# Stock-Prediction-DL

### Purpose: 
Developing deep learning models which utililze historical financial stock data in combination with daily aggregated twitter sentiments to determine the stock buy or sell siganl for a given trading day. Three types of deep learning models were used for this task: RNN, LSTM, and GRUs. Trying to understand the role of social sentiments today when predicting the signal of Microsoft and Tesla. 

### Repository Structure: 
This repository contains the following:

* datasets
    * raw 
        * Contains raw extracted tweets for each year from 2017 to 2020 for Microsoft and Twitter
    * msft-tweet-sentiments-lstm.csv
        * Contans the daily aggregate sentiment scores after classifying each Microsft tweet using the sentiment analysis model
    * msft-tweet-sentiments-lstm.csv
        * Contans the daily aggregate sentiment scores after classifying each Tesla tweet using the sentiment analysis model

* src
    * Microsoft Models
        * Source code for LSTM, RNN, and GRU models which predict the Microsoft stock signals for a given trading day 
    * Sentiment Analysis Model 
        * Source code for bidirectional LSTM model used to generate generate sentiment scores for tweets from Microsoft and Tesla
        * This model was trained using the Sentiment140 training dataset created by created by Alec Go, Richa Bhayani, and Lei Huang, who were Computer Science graduate students at Stanford University. (Link to site here: http://help.sentiment140.com/home)
    * Tesla Model 
        * Source code for LSTM, RNN, and GRU models which predict the Tesla stock signals for a given trading day 
    * Twitter Scraping 
        * Source code for scraping twitter using snscrape library's twitter scraper module (Link to creator's repo here: https://github.com/JustAnotherArchivist/snscrape)
