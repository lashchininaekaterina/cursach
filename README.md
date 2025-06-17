# Analysis of the News Impact on Business

**Author:** Ekaterina Lashchinina  
**Group:** БПАД234  
**Supervisor:** Daria Bashminova  
**Institution:** Higher School of Economics, Faculty of Computer Science  
**Year:** 2025

---

## Project Overview

This project examines the effect of news on stock prices of major Russian firms between 2019 and 2023.
By using NLP tools and statistical data analysis, it identifies patterns of news sentiment and company name mentions that influence market action and stock price movements.

The goal is to empower investors and analysts to better understand the relationship between news and financial indicators so they can make more effective investment decisions.

---

## Features

- News and stock data collection and pre-processing for Russian companies
- News story sentiment analysis
- Correlation analysis of stock prices and sentiment of news, as well as mentions frequency
- Determination and analysis of most important dates when important movement in the stock market was experienced
- The visualization utilities like wordclouds and bigram extraction
- Key entity recognition with SpaCy to extract important people, entities and places on significant dates

---

## Data Sources

- News data collected from Lenta.ru (https://lenta.ru/)  2019-2023  
- Stock price data for big Russian companies downloaded  from the Moscow Exchange website

---

## Methodology

1. **Data Collection and Preprocessing:**
After collecting data from Kaggle and downloading stock data from MOEX and previewing, standardizing date formats in datasets and removing invalid stock prices (zero values ​​on weekends/holidays)

2. **Sentiment Analysis:**
Based on patterns and keywords, news stories were divided into 6 categories: positive, negative, neutral, business positive, and business negative

3.**Data Integration:**
Merging news data with stock prices by date and for each company individually

4. **Correlation Analysis:**
Correlation computation between news sentiment measures and stock prices, and how often each company appears in news. 

5. **Critical Date Analysis:**
News released on critical dates with steep decreases or peaks extraction and analysis close to them in stock market prices with the use of word clouds, bigrams, and key mention extraction

6. **Named Entity Recognition:**
Applying SpaCy for extracting and counting mentions of key entities from news texts.

---
## Results

- Business related news have quite affect significantly stock prices for about one-third of all studied companies.
- The general news also has influence on most companies.
- Frequency of company mentions will be positively correlated with stock price changes in certain companies but will be weak or negative for others.
- Critical date analysis was used to approximately identify market-moving events.
- NLP tools improved understanding of news impact on market conditions.

---

**Limitations**
The analysis is limited to the period from 2019 to 2023, which may prevent us from detecting long-term trends. Computational and time constraints have also affected the amount of data processing and modeling. In addition, we have no experience working with natural language processing (NLP) models.

---

**Future work**
In the future, it will be possible to automate the process of analyzing news in real time for prompt decision-making by analysts and investors, and also to use this method on larger volumes of data. In addition, it will be possible to identify events that are more likely to collapse the stock market or raise it, so that you can be prepared to solve these problems.

---

Technologies used:
Python 3, Pandas, and NumPy were used to collect and process the data. Matplotlib and WordCloud were used for visualization. For NLP, we used the Space and Named Entity Recognition tools to analyze the text.

---

The process of data collecting, data preparation, and obtaining results can be seen in the code located in the file main-2-3.ipynb
