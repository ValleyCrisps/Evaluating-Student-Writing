# Evaluating-Student-Writing

## Kaggle competition page
https://www.kaggle.com/c/feedback-prize-2021/overview

---

## Input data

## Goal

## Assumptions
- Discourses consiste of whole sentences.
- Discourses consist of adjacent sentences.

## Conventions

---

## Proposed approach
1. Split text files into sentences
2. Aggregate sentences into discourses
  For each sentence S, compare S with all sentences in previous discourse and check for logical connections. 
  If a connection is found: add S to current discourse. 
  Else: create new discourse containing and add S to it
3. Apply ML (Machine Learning) algorithms to identify the type of each discourse

---

## NPL (Natural Language Processing) pipeline
1. Data segmentation
  given a text file, split it into smaller units (e.g. sentences)
2. Cleaning
3. Vectorization
  transform sentences into numerical data (e.g. bag of words, N-graphs)
4. Machine learning
5. Interpretation
  compare the results obtained from the machine learning step against expected results

### 1 Data segmentation

### 2 Cleaning
YES
- correct misspelled words
- expand contractions (e.g. they're -> they are)

MAYBE
- remove punctuation
- lemmatization and/or stemming (e.g. cheered -> cheer)
- remove numbers

NO
- all lowercase

### 3 Vectorization
Numberphile video
<https://www.youtube.com/watch?v=gQddtTdmG_8>

### 4 Machine learning
**Random forest**
Basic introduction and tutorials
<https://builtin.com/data-science/random-forest-algorithm>
<https://www.analyticsvidhya.com/blog/2021/06/understanding-random-forest/>

Wikipedia article
<https://en.wikipedia.org/wiki/Random_forest>

Python library
<https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html>

**Cosine similarity**
Basic introduction and tutorials
<https://www.machinelearningplus.com/nlp/cosine-similarity/>

Wikipedia article
<https://en.wikipedia.org/wiki/Cosine_similarity>


**Naive Bayes**
Basic introduction and tutorials
<https://www.geeksforgeeks.org/applying-multinomial-naive-bayes-to-nlp-problems/>

Wikipedia article
<https://en.wikipedia.org/wiki/Naive_Bayes_spam_filtering>

Python library
<https://scikit-learn.org/stable/modules/naive_bayes.html>


**Transformers**


### 5 Interpretation
