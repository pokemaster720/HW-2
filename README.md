# HW-2
Question 1

code was done on Jupyter Notebook

This code is designed to perform a K-Nearest Neighbors (KNN) machine learning algorithm on a set of email data to classify emails as spam or not spam. 
It splits the process into several steps
-data preparation 
-model training 
-prediction 
-evaluation. 

Initial Setup and Data Loading
1. **Importing Libraries**:
   The code starts by importing necessary libraries.
   `pandas` is used for data manipulation,
   `numpy` for numerical computations,
   `Counter` from `collections` is used for counting occurrences of elements, helpful in voting for the most common class in KNN predictions.
   
3. **Loading Data**:
   Data is loaded from `spam_train.csv` and `spam_test.csv` using `pandas`,
   This dataset contains features extracted from emails along with a class/label indicating whether an email is spam (`1`) or not spam (`0`).

 4. ###Data Preparation
- The features (X) and labels (y) are separated for both training and test sets.
- Training features are extracted using `spam_train.iloc[:, 0:56]` (all rows and the first 56 columns assuming the last column is the label)
- labels are extracted from the `class` column. 

 5. ### Model Training (KNN) and Predictions
The core of this code revolves around a manual implementation of the KNN algorithm, which involves:
  1. **Defining a training function**: simulates model training, but in the context of KNN
   
2. **`predict_knn` Function**: A crucial part of this code that seems to compute the distance between a test sample and all training samples to find the nearest neighbors but lacks the final step to return the most common label among the k-nearest neighbors.
Q1
<img width="1220" alt="Screenshot 2024-03-03 at 2 53 53 AM" src="https://github.com/pokemaster720/HW-2/assets/84993132/09bf9f90-8715-4ffd-be3c-3e71f5fdf6cf">

Q3

<img width="755" alt="Screenshot 2024-03-03 at 4 02 59 PM" src="https://github.com/pokemaster720/HW-2/assets/84993132/ca52d943-ebd2-4ab7-8a29-eb90cdd38cf8">
