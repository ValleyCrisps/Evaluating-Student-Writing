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
GOAL: indentify discourses
1. Split text files into sentences
2. Aggregate sentences into discourses
  -> for each sentence S, compare S with all sentences in previous discourse and check for logical connections. 
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

### 4 Machine learning
- Random forest
- Cosine similarity
- Naive Bayes

### 5 Interpretation
