# K-Nearest Neighbours (KNN) Algorithm

This repo provides the implementation of the k-Nearest Neighbors (k-NN) algorithm from scratch using Python. We explore different values of k and visualize the decision boundaries on the two moons dataset.

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
