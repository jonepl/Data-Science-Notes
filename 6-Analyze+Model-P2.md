# Analyze + Mode Part 2

## Predictive Modeling with Machine Learning


### Terminology
---

**Training data** - data you use to train a machine learning alogrithm
    - Input features data (Predictors)
    - Output features data (Response, Outcome)

**Supervised data** - training data that contains Input and Output features 

**Supervised Learning Problems** - is a machine learning task of learning a function that maps an input to an output data based on example input-output pairs (ie Supervised data).

Examples of Supervised Learning models

- Regression model - Output is a *continuous* variable | requires the prediction of a quantity 
- Classification model - requires that examples be classified into *one of two or more classes*. Example Titanic dataset Survived (1) or Not Survived (0)


**Unsupervised data** - training data that only contains Input features data 

**Unsupervisored Learning Problems** - the goal is to identify meaningful patterns in the training data which doesn't contain output data

Examples of Unsupervised Learning models

- K-means clustering
- Reinforcement learning

**Classification Task** - requires that examples be classified into *one of two or more classes*. Example Titanic dataset Survived (1) or Not Survived (0)

Types of Classification Tasks
- Binary Classification Problem -  Judge by accuracy, other precision, recall
- Multi-label Classification
- Classification Predicitive

## Determining Performance

Confusion Matrix - is a table that is often used to describe the performance of a classification model. Use the following table to determine metric performanance.

```
                     Confusion Matrix

+-----------------+---------------------+---------------------+
|                 | Predicted Negative  | Predicted Positive  |
+-----------------+---------------------+---------------------+
| Actual Negative | True Negative (TN)  | False Positive (FP) |
+-----------------+---------------------+---------------------+
| Actual Postive  | False Negative (FN) | True Positive (TP)  |
+-----------------+---------------------+---------------------+
```


Examples of Performance metrics

* Precision (aka Positive Predictive Value) - What proportion of positive identifications was actually correct?
    ```
    Precision = TP/ (TP + FP)
    ```

* Recall - What proportion of actual positives was identified correctly?
    ```
    Recall = TP/ (TP + FN)
    ```

- Accuracy - the percentage of correct predictions for the test data

    ```
    Accuracy = (TP + TN) / (TP + TN + FP + FN)
    ```

- Negative Predictive Value (NPV) - ?

    ```
    NPV = TN/(TN + FN)
    ```

- Sensitivity - True Positive Rate. The proportion of actual negatives, which got predicted correctly

    ```
    Sensitivity = TP/(TP+TN)
    ```

- Specifictiy - True Negative Rate. The proportion of actual negatives, which got predicted correctly
    ```
    Specifity = TN/(TN + FP)
    ```

## Evaluating Your Classifier

If you are given supervised test data you can perform an 80% 20% split in order to train your alogrithm.

1. Split supervised data into 80/20 split
2. Use the 80% supervised data to train a model
3. Use the 20% supervised data to test your tranined model
4. Compare your Predicted Output of you 20% supervised data input to the actual values and determine your score (Precision, Recall)

![Classifier Evaluation](Classifier-Evaluation.png)

---
This idea of a feature is a detail of the data

Statistical modeling is a subfield of mathematics that seeks out relationships between variables in order to predict an outcome.

**Classifier** - a type of machine learning algorithm used to assign a *class label* to a data input

- Logistic Regression
- Support Vector machine
- Neural Networks
- Random forest