---
title: "Predation Machine Learning"
excerpt: "This project involves identifying predatory behaviors in mental health apps using training data to generate a model for analyzing large datasets of user reviews.
<br/><img src=''>"
collection: portfolio
---

# Overview

We previously conducted a qualitative thematic analysis of user reviews left on mental health apps on the Google Play Store, developing a codebook with five categories and nine subcodes. We noted that ~6% of reviews contained descriptions of predatory monetary practices implemented by app developers (see table).

Using these coded reviews, we split our dataset of 10k reviews into training, tuning, and test sets and used various machine learning techniques (Naive Bayes, Support Vector Machines, Decision Trees, Multilayer Perceptrons, and TensorFlow) to attempt to automatically classify predatory reviews. We first focused on binary classification (yes/no predation), and will move on to the subcodes in the future.

## Problem
* Can we use machine learning to identify predatory content described in user reviews of mental health apps?

## Algorithms Implemented
Used the Scikit learn Python library (free machine learning library) to implement the following supervised learning algorithms:
* Naive Bayes
  * Applies Bayes theorem
  * Assumes words in a sentence are independent of each other (independence among predictors)
  * High success rate in text classification
  * Assumes independence among predictive features

* Support Vector Machines
  * Widely used for classification
  * Works well even with limited data 
  * Plots each item then finds the decision boundary to separate the two classes
  * Want this separation to be as wide as possible

* Decisions Trees
  * Models decisions in tree-like structure
  * Conditions split tree into branches

## Results
* Naive Bayes
  * Lowest accuracy and precision
  * High recall - categorized predatory reviews well
* Support Vector Machines
  * Similar to decision trees, but better
  * Worse recall
* Decision Trees
  * High precision, low recall



