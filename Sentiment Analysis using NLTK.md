# Sentiment Analysis using NLTK

## Video link: [Sentiment Analysis using NLTK]()

Sentiment analysis can help you determine the ratio of positive to negative engagements about a specific topic. You can analyze bodies of text, such as comments, tweets, and product reviews, to obtain insights from your audience. In this tutorial, you’ll learn the important features of NLTK for processing text data and the different approaches you can use to perform sentiment analysis on your data.

## Getting Started With NLTK
The NLTK library contains various utilities that allow you to effectively manipulate and analyze linguistic data. Among its advanced features are text classifiers that you can use for many kinds of classification, including sentiment analysis.

Sentiment analysis is the practice of using algorithms to classify various samples of related text into overall positive and negative categories. With NLTK, you can employ these algorithms through powerful built-in machine learning operations to obtain insights from linguistic data.

## Installing and Importing
```
$ python3 -m pip install nltk

import nltk

nltk.download()
```

## Compiling Data

```
words = [w for w in nltk.corpus.state_union.words() if w.isalpha()]
stopwords = nltk.corpus.stopwords.words("english")
words = [w for w in words if w.lower() not in stopwords]

```

