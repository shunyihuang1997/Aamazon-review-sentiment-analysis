# Crypto Currency Analysis
## I)Introduction
---
This project mainly focus on analyzing reviews on Amazon which can help company to find the best product and know which one to be improved


## II)Getting Started
---
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.


- Prerequisites
    You will need a tool to run the program on your local machine such as:
    > VScode, Jupyter Note Book......

 
- Installing
    There are some packages that you will be using:
    > Pandas, Numpy, Matplotlib.pyplot, Seaborn, Scikit-learn(sklearn), bokeh, keras, pmdarima
    - Install packages on Jupyter NoteBook:
      > !pip install 'package name'


- Run the program
    The only thing you will need to do to run the test is input a CSV file with header 
    >[number, Name_of_currency, Symbo_of_currency, Date, High, Low, Open, Close, Volumn, Marketcap]


## III) Methodology
---
- Raw Data:
  
  The dataset was extracted from Kaggle from learning and practicing purposes


- Data pre-processing

To start with, I got the number of each word uses in this dataset, and then the character count. Following with the most important part in NLP which is tokenizing words. Then, I cleaned those words by removing 
stop words in NLTK English, weird symbols, as well as lowing those words to keep them united.

- Data visualization
  
 One important feature in NLP is the word cloud. It is used to represent text data in which the size of each word indicates its frequency or importance. Another key point is to split reviews based on their scores. Since it is
hard to get insight by mixing positive and negative reviews together. Thus, after labling the sentiment, we could split them into positive word cloud and negative word cloud.
Another meaningful plot we could get is from bag of N-Gram. In short, it is a model that represents text document as an unordered colelctions of its n-grams. For example, we could plot out the top K frequency of 
N-grams(N consecutive) words. Moreover, we could separate the review by positive and negative and thus get more insights

- Training Process:

  Used 75% of the data for training purposes, and 25% of the data for testing set.
  In this project, I used modles like logistic regression, decision tree and random forest. 


- Testing

  Each model has been tested on the test set. Besides, we have some other measurement such as AUC-ROC curve, precision and recall rate 


### model 1 : logsitic regression
  - train, test split
  - Used on BOW tokenized trainning set and TFIDF 
  - Applied AUC-ROC curve, precision and recall rate to check the accuracy of the model 

### model 2: Decision tree
  - train, test split
  - Used on BOW tokenized trainning set and TFIDF 
  - Applied AUC-ROC curve, precision and recall rate to check the accuracy of the model 


### model 3: Random forest
  - train, test split
  - Used on BOW tokenized trainning set and TFIDF 
  - Applied AUC-ROC curve, precision and recall rate to check the accuracy of the model 



