# Blockchain NLP
![Image Credit:Bahrain This Week.com](images/ai-blockchain.jpeg)

## Determined Our Source Data & Environment
- Twitter's API
- Built the project in Jupyter Lab
- [Google Slides presentation](https://docs.google.com/presentation/d/1iUyEHhSnRBL9jjJk1DSg_f3G2os2I2VMZiwFwZWFQt4/edit#slide=id.gd5b15f0a3_5_26)


## Project Goals- The main aim is to predict whether the bitcoin would rise or decline using the bitcoin based news.
- Pedict whether the bitcoin would rise or decline using the bitcoin based news.
- Analyze the sentiment of these news and check their correlation with bitcoin prices.

---
## Loaded In and Cleaned the Data
- Compared daily exchange and price differences between Bitcoin to USD
- Mixed external news with crypto data
- Joined the data into a single dataframe

## Data Preparation
- Tokenized the news data
- Apply Lemmatization on the data
- Split the data into test and train
- Built a Random Forest Model

## Data Analysis
- Extracted news that was grouped on daily basis and the target variable was generated using the closing and opening prices.
- Target variable could take either '1' or '0', 1 meaning increase or no change, wherease '0' meaning decline in bitcoin price.  
- Word2Vec was used to convert the news into vectors, so that they could be used to make predictions
- Generated the sentiment using nltk vader based sentiment analyzer.
- Aplied lemmatization to the news to improve the accuracy of sentiment analysis. 

---
## Dashboard
- .

## Conclusions & Predictions
- Very small correlation between the sentiment of the news and the trend in bitcoin prices
- Develop another model with better accuracy because we had a high MSE
- RandomForest Model was used to predict the trend in bitcoin prices and we achieved an accuracy of 95%

## Future Considerations
- Combine Google Trends, OpenBlender and Twython data
- Add more data sources 
- Add news related to other keywords

## Technical Requirements
- Python 3
- Libraries (Pandas, Numpy, OpenBlender, Matplotlib, Seaborn, NLTK, Sklearn)

---
### Resources

- [OpenBlender](https://openblender.io/#/my_dashboard)
- [Gensim](https://www.geeksforgeeks.org/nlp-gensim-tutorial-complete-guide-for-beginners/)
- [AIM](https://analyticsindiamag.com/how-to-use-openblender-the-leading-data-blending-tool/)
- [Google Trends](https://towardsdatascience.com/google-trends-api-for-python-a84bc25db88f)
- [Twitter Dashboard](https://developer.twitter.com/en/portal/dashboard)
- [Atoti - Twitter sentiment](https://www.atoti.io/how-im-failing-my-twitter-sentiment-analysis-for-cryptocurrency-prediction/)
- [Drabble / Twiiter Sentiment and Cryptocurrencies](https://github.com/Drabble/TwitterSentimentAndCryptocurrencies)
- [Computational Methods in the Civic Sphere](http://2017.compciv.org/guide/topics/python-nonstandard-libraries/twython-guide/twitter-twython-api-basics.html#exploring-the-basics-of-the-twitter-api-with-twython)
