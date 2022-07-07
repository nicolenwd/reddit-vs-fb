# Reddit vs FB: Comparing sentiment towards COVID-19 restrictions in Singapore

This repo contains data and scripts used in my thesis for Columbia University's Masters in Quantitative Methods in the Social Sciences (QMSS). My thesis aims to investigate if there is a difference between sentiment towards the tightening of COVID-19 restrictions in Singapore on Reddit vs Facebook, with the hypothesis that Reddit comments would be more negative (i.e. anti-restrictions) compared to Facebook comments.

## Methodology
My project involves the following key stages:    
1. *Data Extraction*: Selecting the relevant Reddit and Facebook posts, then using APIs to scrape comments from the posts.
2. *Text pre-processing*: Applying a variety of NLP methods to pre-process the text for sentiment analysis such as text cleaning, tokenisation, stop words removal, lemmatisation/stemming, text correction, negation handling, emoticon handling, etc. Singlish words in the text will also be specially treated.
3. *Sentiment Analysis*: Applying and evaluating the performance of singular/ensemble sentiment analysis algorithms/models like VADER, TextBlob, Afinn, NLTK, spaCy, etc.
4. *Statistical Analysis*: Using R statistical packages to compute the mean sentiment polarity score for each Reddit and FB comment sample, followed by a Welch t-test to determine if there is a statistically significant difference in sentiment of each sample.
5. *Trend Analysis*: Adding a temporal dimension to the analysis by investigating how sentiment on Reddit and FB converge/diverge over time and in relation to key developments (e.g. new variants like Delta/Omicron) and changes in the number of COVID-19 cases in Singapore.

## Code
- *scripts/extract_reddit.ipynb* – a Python script that scrapes data from selected Reddit posts using the [Pushshift Reddit API](https://github.com/pushshift/api).
- *scripts/extract_fb.ipynb* - a Python script that scrapes data from selected FB posts using the [facebook-scraper](https://pypi.org/project/facebook-scraper/) Python package.
- *data* - a folder containing extracted Reddit/FB comment data, and (incoming) sentiment analysis output.

## Author
Nicole Neo, [nicolenwd](https://github.com/nicolenwd)
