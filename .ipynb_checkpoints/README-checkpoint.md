# Crypto Sentiment
![Image Credit:Bahrain This Week.com](images/ai-blockchain.jpeg)

## Determined Our Source Data & Environment
- [Twitter API](https://developer.twitter.com/en/portal/dashboard)
- [OpenBlender API](https://openblender.io/#/my_dashboard)
- [Google Trends Data](https://towardsdatascience.com/google-trends-api-for-python-a84bc25db88f)
- Built the project in Jupyter Lab
- [Google Slides presentation](https://docs.google.com/presentation/d/1iUyEHhSnRBL9jjJk1DSg_f3G2os2I2VMZiwFwZWFQt4/edit#slide=id.gcb9a0b074_1_0)
- Pip Install - Pytrends, Pandas_DataReader, OpenBlender, Gensim, Wordcloud 
- Full import list of libraries and dependencies is below the Resources

## Project Goals
- Predict whether Bitcoin would rise or fall based on Bitcoin news.
- Analyze the sentiment of this news and it's correlation with bitcoin prices.

## Loaded In and Cleaned the Data
- Compared daily exchange and price differences between Bitcoin and USD.
- Mixed external news with crypto data.
- Joined the data into a single dataframe.

## Data Preparation
- Tokenized the news data.
- Applied Lemmatization to the data.
- Split the data into test and train.
- Built a Random Forest Model.

## Data Analysis
- Extracted news that was grouped on daily basis and the target variable was generated using the closing and opening prices.
- Target variable could take either '1' or '0', 1 meant an increase or no change, whereas '0' meant a decline in bitcoin price.  
- Word2Vec was used to convert the news into vectors so that they could be used to make prediction.
- Generated the sentiment using NLTK Vader based sentiment analyzer.
- Applied lemmatization to the news to improve the accuracy of sentiment analysis. 

## Dashboard
![Google Trends hits](images/google_trends.png)
![Google Trends Data](images/google_trends_data.png)
![Wordcloud](images/count_target_labels.png)
![Wordcloud](images/wordcloud.png)

## Conclusions & Predictions
- Small correlation between the sentiment of the news and the trend in bitcoin prices.
- RandomForest Model was used to predict the trend in bitcoin prices and we achieved an accuracy of 95%.

## Future Considerations
- Develop another model with better accuracy because we had a high MSE.
- Combine Google Trends, OpenBlender and Twython data.
- Add more data sources and other keywords to the analysis.

## Technical Requirements
- Python 3
- Libraries (Pandas, Numpy, OpenBlender, Matplotlib, Seaborn, NLTK, Sklearn)

### Resources

- [OpenBlender](https://openblender.io/#/my_dashboard)
- [Gensim](https://www.geeksforgeeks.org/nlp-gensim-tutorial-complete-guide-for-beginners/)
- [AIM](https://analyticsindiamag.com/how-to-use-openblender-the-leading-data-blending-tool/)
- [Google Trends](https://towardsdatascience.com/google-trends-api-for-python-a84bc25db88f)
- [Twitter Dashboard](https://developer.twitter.com/en/portal/dashboard)
- [Atoti - Twitter sentiment](https://www.atoti.io/how-im-failing-my-twitter-sentiment-analysis-for-cryptocurrency-prediction/)
- [Drabble / Twiiter Sentiment and Cryptocurrencies](https://github.com/Drabble/TwitterSentimentAndCryptocurrencies)
- [Computational Methods in the Civic Sphere](http://2017.compciv.org/guide/topics/python-nonstandard-libraries/twython-guide/twitter-twython-api-basics.html#exploring-the-basics-of-the-twitter-api-with-twython)
- [Vector Stock](www.vectorstock.com)

### Libraries & Dependencies
- import pandas as pd
- import numpy as np
- from numpy import concatenate
- import OpenBlender
- import json
- import seaborn as sns
- import datetime as dt
- from Data import Data
- import math
- from math import sqrt
- from pandas import DataFrame
- from pandas import concat
- import nltk
- from nltk.stem import WordNetLemmatizer
- from nltk.corpus import wordnet
- nltk.download('vader_lexicon')
- from nltk.sentiment.vader import SentimentIntensityAnalyzer
- import gensim
- from sklearn.ensemble import RandomForestClassifier
- from sklearn.model_selection import train_test_split
- from sklearn.metrics import f1_score,accuracy_score
- from sklearn.ensemble import RandomForestRegressor
- from sklearn.preprocessing import MinMaxScaler
- from sklearn.metrics import r2_score
- from sklearn.metrics import mean_squared_error, r2_score
- from wordcloud import WordCloud
- import matplotlib.pyplot as plt
- plt.style.use('seaborn-whitegrid')
- import matplotlib as mpl
- mpl.rcParams['figure.figsize'] = [20.0, 10.0]
- %matplotlib inline
- from matplotlib import pyplot as plt
- from tensorflow.keras import Sequential
- from tensorflow.keras.layers import LSTM, Dense, Dropout, Activation
- from pandas import read_csv
- from GoogleTrendAPI_Direct import GoogleTrendAPI



