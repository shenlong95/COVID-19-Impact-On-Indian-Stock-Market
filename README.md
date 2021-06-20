# Impact of COVID-19 On Indian Economy from the Perspective of Indian Stock Market.  
# [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/) [![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try) [![Binder](https://binder.pangeo.io/badge_logo.svg)](https://mybinder.org/v2/gh/strikersps/COVID-19-Impact-On-Indian-Stock-Market/HEAD)

[![GitHub contributors](https://img.shields.io/github/contributors/strikersps/COVID-19-Impact-On-Indian-Stock-Market.svg)](https://GitHub.com/strikersps/COVID-19-Impact-On-Indian-Stock-Market/graphs/contributors/)
[![GitHub Issues](https://img.shields.io/github/issues/strikersps/COVID-19-Impact-On-Indian-Stock-Market)](https://github.com/strikersps/COVID-19-Impact-On-Indian-Stock-Market/issues)
[![GitHub Stars](https://img.shields.io/github/stars/strikersps/COVID-19-Impact-On-Indian-Stock-Market)](https://github.com/strikersps/COVID-19-Impact-On-Indian-Stock-Market/stargazers/)
[![GitHub Forks](https://img.shields.io/github/forks/strikersps/COVID-19-Impact-On-Indian-Stock-Market)](https://github.com/strikersps/COVID-19-Impact-On-Indian-Stock-Market/network/members)
[![Dalal Street Image](https://github.com/strikersps/COVID-19-Impact-On-Indian-Stock-Market/blob/main/Dalal-Street.jpg)](https://www.bloombergquint.com/markets)

**NOTE:** Do run the jupyter notebook name [`Impact_of_COVID_19_on_Indian_Stock_Market.ipynb`](https://mybinder.org/v2/gh/strikersps/COVID-19-Impact-On-Indian-Stock-Market/HEAD) after running the docker image from the above link again by going into `Kernel` dropdown in the taskbar and select `Restart & Run All` in order to see all the visualizations.

### Objective
This project is an analysis based on the publicly available datasets related to COVID-19, Indian Stock Market Indices Dataset, Volatility Prices and Oil Prices. The goal is to examine the behaviour of Indian Stock Market from Jan 2020 to Dec 2020 and how it was impacted due to COVID-19, Oil Price War between Russia and Saudi Arabia, Lockdowns due to COVID-19 and other major events happened during the period.  

### Introduction
* Indian stock market saw one of the biggest falls in its history i.e. **BSE SENSEX and NIFTY-50 corrected sharply by 38% in March 2020**, more specifically this crash was another major crash after the Global Financial Crisis of 2008 which was due to fall in the Housing Price in the USA.
* COVID-19 had a brutal and dramatic impact on financial markets all over the world. It has exposed investors to unprecedented levels of risks causing investors all over the world to suffer significant losses in a very short period of time. 

* The idea was that if you want to measure/gauge the behaviour of the stock market then you look at the different indices listed in the exchanges as indices are the best way to measure how the whole market or a section/sector of the market is performing. Market indices are classified on the basis of broader/benchmark market indices and sector indices majorly and every exchange has its own set of indices.
* Indian Stock Market has two major exchanges namely National Stock Exchange and Bombay Stock Exchange and there are more than 5000 companies listed on both the exchanges and monitored by the market regulator SEBI. So to gauge the market we need to look at the price action of benchmark indices and sector indices. There are various indices but the most famous and concise indices are SENSEX of Bombay Stock Exchange(BSE) and NIFTY-50 of National Stock Exchange(NSE). There is another index known as INDIA VIX which is a way to gauge the volatility in the Indian market. Volatility is a very important variable in order to understand whether on a given market session or time period the investors are afraid or greedy when buying securities in the market.  
* The stock market in the short term can be considered as a sentiment index of an economy and it's a way to measure the emotions of an economy. If you look at the stock market benchmark indices after March 2020, you will see a very quick recovery in the market and selected sectors like IT, Pharmaceuticals due to which it is hard to answer the question whether COVID-19 has impacted the market or not just on the basis of data?  
* The main goal of the project is to identify/quantify the relationship between the COVID-19 and other major events which are a direct or indirect consequence of COVID-19 and its impact on the Indian Economy by studying, visualising, and establishing relationships between the Indian Stock Market Indices (NIFTY-50 and SENSEX), COVID-19 cases and deaths around the world, lockdowns imposed by the governments and various other events.

* This report stays away from making prediction on Indian financial markets because a huge proportion of Indian economy is unorganized. With limited time and infrastructure, it is really hard to make any short term predictions of the stock market because upside and downside in a short term or long term depends upon various factors like economic, social, technology, climate, businesess etc.

* **The efficient-market hypothesis (EMH) is a hypothesis in financial economics that states that asset prices reflect all available information. A direct implication is that it is impossible to "beat the market" consistently on a risk-adjusted basis since market prices should only react to new information. The idea that financial market returns are difficult to predict goes back to [Bachelier (1900)](https://en.wikipedia.org/wiki/Efficient-market_hypothesis#cite_note-3), [Mandelbrot (1963)](https://en.wikipedia.org/wiki/Benoit_Mandelbrot), and [Samuelson (1965)](https://en.wikipedia.org/wiki/Paul_Samuelson), but is closely associated with [Eugene Fama](https://en.wikipedia.org/wiki/Eugene_Fama), in part due to his influential 1970 review of the theoretical and empirical research.**

### Datasets
* For the project I have extracted the datasets of price actions of SENSEX, NIFTY50, INDIA VIX, COVID-19 Total Deaths and Cases Worldwide, and also the price actions of some of the sector indices which are heavily impacted due to COVID-19 i.e. NIFTY-AUTO, NIFTY-IT, NIFTY-PHARMA, NIFTY-BANK, NIFTY-MEDIA, NIFTY-REALTY, NIFTY-FMCG.
* As the Oil Price War between Saudi Arabia and Russia has also impacted the market I have also used the Crude Oil WTI and BRENT Europe Price Data with CBOE-Crude-Oil Volatilty dataset. 
* For some of the datasets I have used a python library `Quandl` which provides access to price actions of various financial securities/instruments as described in the above cells.

* Following table shows a summary of all the datsets with their source:

| Sr.No | Name of Dataset | Source |
| --- | --- | --- |
| 1 | COVID-19-Dataset | [Our World In Data COVID-19 Dataset](https://github.com/owid/covid-19-data/tree/master/public/data) |
| 2 | Crude Oil WTI Price Index | Fetched through `quandl`|
| 3 | BRENT Europe Crude Oil Price Index| Fetched through `quandl`|
| 4 | VIX index of OVX (ETF on Crude Oil)| [CBOE Crude Oil Volatility Index (^OVX)](https://finance.yahoo.com/quote/%5EOVX/)|
| 5 | INDIA-VIX | [INDIA-Volatility Index (INDIA VIX)](https://www1.nseindia.com/products/content/equities/indices/historical_vix.htm)|
| 6 | NIFTY-50 | [NIFTY-50-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 7 | BSE-SENSEX | Fetched through `quandl`|
| 8 | NIFTY-IT | [NIFTY-IT-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 9 | NIFTY-PHARMA| [NIFY-Pharma-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm) |
| 10 | NIFTY-FMCG | [NIFTY-FMCG-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 11 | NIFTY-Auto | [NIFTY-Auto-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 12 | NIFTY-Media| [NIFTY-Media-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 13 | NIFTY-Bank| [NIFTY-Bank-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 14 | NIFTY-Realty| [NIFTY-Realty-Index-Data](https://www1.nseindia.com/products/content/equities/indices/historical_index_data.htm)|
| 15 | Google Trends | Fetched using `pytrends` |

**NOTE**
* The datasets listed above are final datasets (subject to change as it is a time-series) data.
* I have not included one more dataset on which I am working on i.e. Twitter Dataset as it requires more time in order to implement Association Rule Mining algorithm to find out words people are most using whenever they tweet during the COVID-19 period.

### Future Works
* The best way to measure the sentiment of the people is by doing the association rule mining and sentiment analysis of tweets written by people all around the world on twitter during this time period because almost every politician, CEOs, leaders etc are on twitter and they use it as a platform to convey their views.

* After doing twitter sentiment analysis and relating it to the fall of the market may give me an opportunity to publish a research paper and make my work presentable in the researh community.

### Conclusions
* The main conclusions drawn from the above work are: 
    * **Market was reacting to the anticipation and the consequences of Globalization.** The market downturn/sharp correction in the global markets was influenced by a non-economic factor/an unpredicted event i.e. COVID-19 Pandemic and it has affected almost all of the major sectors of the global economy. 
    But one more question arises at the same time that how only COVID-19 pandemic has made the market fall by that much, more clearly **Does COVID-19 is the only reason for the fall happened in March-2020?** and the answer is Yes but not just COVID-19 rather the sequence of events or the ripple affect caused by COVID-19 like countries imposing strict lockdown policies, businesses are shutting down their daily operations except the pharmaceutical and consumer discretionary sectors, MSMEs (Micro, Small & Medium Enterprises) are severely affected due to lockdowns, people all around the world were panicking (which is not good) under the impression of Global Recession and at the same time there was an [Oil Price War](https://en.wikipedia.org/wiki/2020_Russia%E2%80%93Saudi_Arabia_oil_price_war) which had happened between Saudi-Arabia and Russia which made the market fall further in the March and April of 2020.  

    * COVID-19 is still present and it is affecting people at a pace but markets all around the world are at all time highs just after the fall of March, 2020 which is a contradiction to my initial hyphothesis which was based upon previous financial crisis i.e. **"It will take atleast 2 years for the market to recover its losses and reach its all-time highs again"** but the opposite has happen. Even though COVID-19 has made the market fall sharply still markets globally recovered quickly in just 8-9 months.  

### License  
[![GPLv3 license](https://img.shields.io/github/license/strikersps/COVID-19-Impact-On-Indian-Stock-Market?style=for-the-badge)](http://perso.crans.org/besson/LICENSE.html) 
