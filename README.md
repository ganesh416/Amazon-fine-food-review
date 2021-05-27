# Amazon-fine-food-review

# over review
Social media has given ample opportunity to the consumer in terms of gauging the quality of the
products by reading and examining the reviews posted by the users of online shopping platforms.
Moreover, online platforms such as Amazon.com provides an option to the users to label a review
as ‘Helpful’ if they find the content of the review valuable. This helps both consumers and
manufacturers to evaluate general preferences in an efficient manner by focusing mainly on the
selected helpful reviews. However, the recently posted reviews get comparatively fewer votes and
the higher voted reviews get into the users’ radars first. This study deals with these issues by
building an automated text classification system to predict the helpfulness of online reviews
irrespective of the time they are posted. The study is conducted on the data collected from
Amazon.com consisting of the reviews on fine food.(using  database sqlite)
 
# text cleaning:
there are varioius technics to text cleaning like stemming, stop words removal, tokenization, lemmitization,Lowercasing,Normalization

# Why text preprocessing ?
As we know Machine Learning needs data in the numeric form. We basically used encoding technique (BagOfWord, Bi-gram,n-gram, TF-IDF, Word2Vec) to encode text into numeric vector. But before encoding we first need to clean the text data and this process to prepare(or clean) text data before encoding is called text preprocessing, this is the very first step to solve the NLP problems.
 
 here  i am using countvectorizer to covert words into vectors and it will used to sentiment analysis
 
# Importing libraries and loading the files
import pandas as pd
import numpy as np
from sklearn import linear_model
from sklearn.externals import joblib
import joblib as jb
import sqlite3
from bs4 import BeautifulSoup
import re
from sklearn.feature_extraction.text import CountVectorizer


#  machine learning model 
linear model:
Linear Regression is a supervised machine learning algorithm where the predicted output is continuous and has a constant slope. It’s used to predict values within a continuous range, (e.g. sales, price) rather than trying to classify them into categories (e.g. cat, dog)
this model train by review data set and score of that review and this model helps to predict whether input query review positive or nagetive




