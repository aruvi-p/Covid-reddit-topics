# Covid-reddit-topics
LDA analysis of topics from Reddit conversations on Covid-19


# Analysis of Reddit Threads on Corona

This notebook primarily focuses on analysing the all the threads and comments under https://www.reddit.com/r/Coronavirus/.
The notebook consists of 8 major parts. 

1. Extraction of the relevant data fields using the Reddit API

2. Cleaning of the text columns and export the data to a json file keeping the relationships through indices

3. Pre-processing the data for topic modelling and frequent words analysis which includes stop words removal, stemming, lemmatizing etc,.

4. Building corpus using Bag of words

5. Building corpus using TF-IDF

6. Plotting two LDA visualizations on the two corpuses

7. Additional visualizations on the topic modelling

8. A simple word cloud based on frequently used words

## Installation

Install the following packages to run the python notebook.

```bash
pip install praw
pip install gensim
pip install nltk
pip install pandas
pip install pyLDAvis
pip install wordcloud 

```

# Analysis of Reddit Threads on Corona

This notebook primarily focuses on analysing the all the threads and comments under https://www.reddit.com/r/Coronavirus/.
The notebook consists of 8 major parts. 

1. Extraction of the relevant data fields using the Reddit API

2. Cleaning of the text columns and export the data to a json file

3. Pre-processing the data for topic modelling and frequent words analysis which includes stop words removal, stemming, lemmatizing etc,.

4. Building corpus using Bag of words

5. Building corpus using TF-IDF

6. Plotting two LDA visualizations on the two corpuses

7. Additional visualizations on the topic modelling

8. A simple word cloud based on frequently used words

## Installation

Install the following packages to run the python notebook.

```bash
pip install praw
pip install gensim
pip install nltk
pip install pandas
pip install pyLDAvis
pip install wordcloud 

```

## Algorithms used and other details:

1. Python Reddit API Wrapper is used to download all the threads from the subreddit "Coronavirus"

2. The extracted columns are Title, score, ID, URL attached, comms numbers, creation date, the body and the comments

3. The text columns are cleaned and the date columns are formatted

4. This cleaned data frame is exported to a .json file

5. Pre-processing is done on the text columns which includes:


--------a) Tokenization: Split the text into sentences and the sentences into words. Lowercase the words and remove punctuation.

--------b) Words that have fewer than 3 characters are removed.

--------c) All stopwords are removed.

--------d) Words are lemmatized — words in third person are changed to first person and verbs in past and future tenses are changed into present.

--------e) Words are stemmed — words are reduced to their root form

6. Corpuses are built on the combined text data using two different packages - Bag or words and Tf-idf

7. Latent Dirichlet allocation model is run on these corpus to arrive at the topics that are being discussed. The output is visualized in an interactive plot

8. Different visualizations are plotted using the topics arrived at using LDA

9. A word cloud is plotted highlighting the most frequently used words in the threads




```
