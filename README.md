# Crypto Currency Sentiment Tracker 

This is a Crypto board website that scrapes data from various news and social media sites,
and displays to the user the graphs and other data in order to gauge popularity of certain cryptos.


## Description of source code
Backend:
- The aggregator module consists of FireBase.py and sentiment_analysis.py.
    - Firebase.py is responsible for establishing the connection between the instance and the Firebase database, as well as getting and setting data. 
    - sentiment_analysis.py is responsible for various tasks, including sentence summarizer, sentiment analyzer, and various text processors 
- The scraper module consists of two types of scrapers - Scrapy for news sources and PRAW for reddit.
    - We use Scrapy to scrape two news sources for data about various cryptocurrencies
    - We use the PRAW library to scrape Reddit's CryptoCurrency subreddit for recent posts and comments that mention a particular cryptocurrency
    
Frontend:
- The frontend was made using React and Vite, and mainly lives in the hosting directory.
- Within the subdirectory are various components necessary to make the frontend, such as firebase, which is responsible for establishing a connection with the database for the frontend.
- The project also includes UI elements, such as tables, buttons, and breadcrumbs, as well as CCS for styling.
