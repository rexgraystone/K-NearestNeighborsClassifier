# K-Nearest Neighbors Classifier with custom algorithm and library implementations

## Problem statement

Build a _k_ nearest neighbor classifier in Python to classify the MNIST digit data. This is a multi-class classification problem with labels from 0 to 9.

## Values

  1. **Number of neighbors _'k'_:** 44

  2. **Number of data points:** 7100

  3. **Testing process** (cross-validation): 1420 (Randomly picking 20% of the data for testing, and doing the testing _k_ many times; each time picking the 20% test data randomly)

## Implementation

Write the code for a custom kNN algorithm, and generate an averaged confusion matrix. Repeat the process using sklearn's KNeighborsClassifier library classifier.

## Anomalies

  1. Sometimes in the Custom kNN classifier, due to losses in the decimal places, when calculating the total number of elements in the final confusion matrix, the answer may not always be the exact number of testing datapoints used, rather it could produce a value that is extremely close to the intended answer.

  2. Since the confusion matrix that we are printing in the end holds the average value, the values of the elements may have decimal places; as it is not necessary that the values add up to a value that is divisible by _k_.

## List of Files

| File Name | Description |
| :---: | :---: |
| [K-Nearest Neighbors Classifier - Custom](https://github.com/rexgraystone/K-NearestNeighborsClassifier/blob/main/K-Nearest%20Neighbors%20Classifier%20-%20Custom.ipynb) | A kNN classifier using a hardcoded algorithm |
| [K-Nearest Neighbors Classifier - Library](https://github.com/rexgraystone/K-NearestNeighborsClassifier/blob/main/K-Nearest%20Neighbors%20Classifier%20-%20Library.ipynb) | A kNN classifier using scikit-learn's library classifier |
| [Documentation](https://github.com/rexgraystone/K-NearestNeighborsClassifier/blob/main/Documentation.pdf) | Documentation of the project |
