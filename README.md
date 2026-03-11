# K-Nearest Neighbors (KNN) from Scratch

This project implements K-Nearest Neighbors (KNN) from scratch using Python and NumPy, without using machine learning libraries such as scikit-learn.

The purpose of this project is to understand how instance-based learning works and how KNN classifies data points based on similarity to nearby data.

## **Overview**

K-Nearest Neighbors (KNN) is a supervised machine learning algorithm used for classification and regression problems It predicts the class of a data point based on the classes of its nearest neighbors.

Unlike many machine learning algorithms, KNN does not learn a model during training Instead, it simply stores the training data and performs calculations when making predictions.

The algorithm works as follows:

1. Choose the number of neighbors k.
2. Calculate the distance between the new data point and all training points
3. Select the k closest neighbors
4. Use majority voting to determine the predicted class

## **Distance Calculation**

This implementation uses Euclidean Distance to measure how close two points are in feature space.
Euclidean Distance formula:

d = √∑(x₁ − x₂)²

Where:
- x₁ = first data point
- x₂ = second data point
- d = distance between the two points

The algorithm computes this distance between the test point and all training points to determine the nearest neighbors.

## **Prediction Process**

To predict the class of a new data point:

1. Calculate distances between the new point and all training data
2. Sort the distances
3. Select the k nearest neighbors
4. Count the labels of those neighbors
5. Assign the label that appears the most (majority vote)

## **Advantages of KNN**
- Simple and easy to understand
- No training phase required
- Works well for small datasets
- Can capture complex decision boundaries
- Flexible for both classification and regression

## **Disadvantages**
- Slow for large datasets
- Requires storing the entire training dataset
- Sensitive to the choice of k
- Performance decreases with high-dimensional data
