# K-Nearest Neighbours (KNN) Algorithm

This README file provides an overview of the `k`-Nearest Neighbours (KNN) algorithm implementation. The KNN algorithm is a simple, yet effective, machine learning algorithm used for classification and regression tasks.

## 1. Implementation of KNN Algorithm

The KNN algorithm has been implemented in Python, following the structure and API of Scikit-Learn. The implementation involves two main steps: training and prediction.

### Training

During the training phase, the algorithm simply stores the training examples \( D = \{(x_i, y_i)\}_{i=1}^{n} \).

### Prediction

To predict the class label for a test point \( x^* \):
1. Calculate the Euclidean distance between \( x^* \) and each training point \( x_i \).
2. Identify the `k` training points with the smallest distances to \( x^* \).
3. Fetch the class labels corresponding to these `k` nearest neighbors.
4. Determine the class label that appears most frequently among these `k` neighbors. In case of a tie, choose the smallest class label deterministically.

### Required Libraries

Install the necessary Python libraries:

```bash
pip install numpy matplotlib scikit-learn
```

### Run

Run the following command:

```bash
python knn_classifier.ipynb
```
