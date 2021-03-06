
# Using NLP Techniques and Text Analytics on Ariana Grande Lyrics 

### Highlights

| <img src="images/semantic_network_new.png" width="500" height="500" />  | 
|:--:| 
| A semantic network of the top 50 words in Ariana's discography |


To view a static version of this notebook, click [here](https://github.com/tatianabarbone/text-analytics/blob/master/text_analytics_ariana_grande.ipynb), or click 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1x2GxmWUc-uERbEl4av0jqz4BmrFKgdIT)  to view this project in a Google Colaboratory notebook.

### Introduction

I've been an Ariana Grande fan since 2013. Since then, she has released six albums (and counting) so I figured over 60 songs would be plenty of data to explore how her lyrics have changed over time.

### Goal

The goal of this project is to use exploratory data analysis to uncover trends in the song lyrics using visualizations of the data. Specifically, I want to answer these questions:

1. How do Ariana Grande's songs and albums differ in terms of sentiment? How are they similar?
2. What are the most frequent words in her songs? Which bigrams does she use the most?
3. How have Ariana Grande's songs changed over time?

### Process

* Retrieves song information by scraping data from the web using requests and BeautifulSoup
* Cleans data
* Structures and mungs data using pandas
* Applies common NLP techniques such as sentiment analysis
* Provides insightful visualizations with matplotlib and Gephi

### About the Data

To get the data I used BeautifulSoup to parse text from two websites: discogs.com and genius.com. I pulled the song titles from discogs and using the song title, made a request to genius for the lyrics of the song. I stored the data in a pandas data frame.

### Conclusion / Results

Through this project, I discovered the most prominent words and bigrams that appear in Ariana’s lyrics. Using sentiment analysis, I found the following:
1. The high and low points in each of her albums 
2. Which albums were similar by sentiment
3. Clusters of similar songs 
4. Songs that were outliers (had drastically different sentiment scores than others)

![lineplot](https://github.com/tatianabarbone/text-analytics/blob/master/images/sentiment_lineplot.png)

Using a co-occurence matrix of keywords I produced a semantic network highlighting clusters of interconnected words. From this we can conlcude that love is an overarching topic in her songs.


### Project Value and Actionable Next Steps

This project helped me understand trends in Ariana Grande's albums, her lexical diversity and how her albums have changed over time.

To add to this project, we can try running ML algorithms on the data to see if we can create a model that accurately predicts the sentiment of any song based on its order in the album or words that are likely to appear in future Ariana Grande albums. We can try to recommend similar songs based on sentiment or try this process on a different artist.

**October 2020 Update:** Ariana released a new album, and I am planning on incorporating lyrics from *Positions* into this project.

**January 2021 Update:** The notebook has been updated to include songs from *Positions*.
