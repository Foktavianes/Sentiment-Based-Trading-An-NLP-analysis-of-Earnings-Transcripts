# Sentiment-Based-Trading-An-NLP-analysis-of-Earnings-Transcripts

The datasets are obtained from WRDS database which is accessed using SQL query. The extracted data are earnings call transcripts for S&P 500 companies which is taken from 2008 until 2023.

There are 4 parts for this projects.
  1. BERT + VADER
     
     I utilized the BERT model to do the tokenization of earnings call transcripts and using the sentence extraction method to obtain the sentence that contain specific words that could imply long or short position. Furthermore, I will implement VADER model to gain sentiment on this sentences and overall earning call transcripts.

  2. FinBERT

     The concept here is similar with above model. The difference is that we used FinBERT model which is known for sentiment analysis for financial instruments. The tokenisation and sentiment will be done with FinBERT model.

  3. Feature Importance Techniques

     This is done to gain insights about how importance is sentiment among other factors in predicting return of the stocks.

  4. Topic Modelling

     I am trying to gain insights on the topic of earning call transcripts within specific sector. This part will comparing combination of LDA and Bag of Words with LDA and TF-IDF.

The last step for this project is to assess the performance of the sentiment generated from BERT + VADER with FinBert. There are 2 rebalancing method and several trading strategies. Based on the backtester, I found out that annual rebalancing method is the better method. Also, the BERTVADER results in annual sharpe of 1.31 if we only consider data that is higher than 50% quantile on sentiment level whereas the FinBERT results in annual sharpe of 1.47 if we only consider data that is higher than 75% quantile on sentiment level.

![image](https://github.com/Foktavianes/Sentiment-Based-Trading-An-NLP-analysis-of-Earnings-Transcripts/assets/112449862/82ed35c1-32d9-4e73-b99e-8835478246c2)
