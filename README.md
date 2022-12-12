## TOPIC MODELLING USING GENSIM-LDA IN PYTHON

### TOPIC MODELLING:

Topic modelling is an unsupervised method of clustering the words for a set of documents. It is refered to as unsupervised because the algorithm clusters without any set of predifined labels. Here, if you feed the model with data, it will produce a set of words which will represent the topic.

### LDA:

LDA’s approach to topic modeling is it considers each document as a collection of topics in a certain proportion. And each topic as a collection of keywords, again, in a certain proportion.

Once you provide the algorithm with the number of topics, all it does it to rearrange the topics distribution within the documents and keywords distribution within the topics to obtain a good composition of topic-keywords distribution.

A topic is nothing but a collection of dominant keywords that are typical representatives. Just by looking at the keywords, you can identify what the topic is all about.

### DATASET

https://raw.githubusercontent.com/selva86/datasets/master/newsgroups.json

### INSTALLATION

>import re

>import numpy as np

>import pandas as pd 

>from pprint import pprint


#### Gensim
>import gensim

>import gensim.corpora as corpora

>from gensim.utils import simple_preprocess

>from gensim.models import CoherenceModel

#### spacy for lemmatization
>import spacy

#### Plotting tools
>import pyLDAvis

>import pyLDAvis.gensim  

>import matplotlib.pyplot as plt

>%matplotlib inline



#### NLTK Stop words
>from nltk.corpus import stopwords
