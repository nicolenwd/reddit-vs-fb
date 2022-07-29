# Reddit vs FB: Comparing sentiment towards COVID-19 restrictions in Singapore

This repo contains data and scripts used in my thesis for Columbia University's Masters in Quantitative Methods in the Social Sciences (QMSS). My thesis aims to investigate if there is a difference between sentiment towards the tightening of COVID-19 restrictions in Singapore on Reddit vs Facebook, with the hypothesis that Reddit comments would be more negative (i.e. anti-restrictions) compared to Facebook comments.

## Methodology
My project involves the following key stages:    
1. *Data Extraction*: Selecting the relevant Reddit and Facebook posts, then using APIs to scrape comments from the posts.
2. *Text pre-processing*: Applying a variety of NLP methods to pre-process the text for sentiment analysis such as text cleaning, tokenisation, stop words removal. Singlish and domain-specific phrases in the text will also be specially treated and replaced with meanings in English.
3. *Sentiment Analysis*: Applying and evaluating the performance of sentiment analysis algorithms like VADER and TextBlob on the comment corpora.
4. *Hypothesis testing*: Computing mean sentiment polarity scores for each Reddit and FB comment sample and conducting appropriate statistical two-sample tests to determine if there is a statistically significant difference in sentiment of each sample. 
5. *Temporal Analysis*: Adding a temporal dimension to the analysis by investigating how sentiment on Reddit and FB converge/diverge over time and in relation to key developments (e.g. new variants like Delta/Omicron) and changes in the number of COVID-19 cases in Singapore.

## Code
- *scripts/0_extract_reddit.ipynb* – Python script that scrapes data from selected Reddit posts using the [Pushshift Reddit API](https://github.com/pushshift/api).
- *scripts/1_extract_fb.ipynb* - Python script that scrapes data from selected FB posts using the [facebook-scraper](https://pypi.org/project/facebook-scraper/) Python package.
- *scripts/2_word_frequency.ipynb* - Python script that obtains word frequencies in the corpora for use in later sentiment analysis.
- *scripts/3_sentiment_analysis.ipynb* - Python script that conducts sentiment analysis using VADER/TextBlob and evaluates the results.
- *scripts/4_further_analysis.ipynb* - Python script that conducts further statistical and temporal analysis on the output for further insights.
- *data* - a folder containing extracted Reddit/FB comment data, cleaned text data and sentiment analysis output.

## Author
Nicole Neo, [nicolenwd](https://github.com/nicolenwd)
