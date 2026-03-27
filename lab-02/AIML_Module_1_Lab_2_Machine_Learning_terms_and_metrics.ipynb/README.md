# 📘 Machine Learning Lab – Lab 2

## Machine Learning Terms and Metrics

---

## 🔹 Objective

The objective of this lab is to understand the basic machine learning pipeline, implement a simple classification model using the California Housing dataset, and evaluate model performance using different metrics.

---

## 🔹 Dataset Description

The California Housing dataset contains:

* **20640 samples (rows)**
* **8 input features**
* **Target variable**: Median house value

Since the target values are continuous, they are converted into integers to perform classification.

---

## 🔹 Steps Performed

### 1. Data Loading

The dataset is loaded using sklearn:

```python
dataset = datasets.fetch_california_housing()
```

---

### 2. Data Preprocessing

The target values are converted from continuous to discrete:

```python
dataset.target = dataset.target.astype(int)
```

---

### 3. Splitting the Data

The dataset is split into:

* Training set
* Validation/Test set

Using a custom split function.

---

### 4. Model Implementation

#### 🔸 1-Nearest Neighbor (1-NN)

* Predicts label based on closest training point
* High training accuracy (overfitting)

#### 🔸 Random Classifier

* Assigns labels randomly
* Used as baseline comparison

---

### 5. Evaluation Metrics

#### ✅ Accuracy

Accuracy = (Correct Predictions) / (Total Predictions)

#### ✅ Confusion Matrix

* Shows actual vs predicted labels
* Diagonal values = correct predictions

---

### 6. Cross Validation

* Multiple splits are performed
* Average accuracy is calculated
* Gives stable and reliable results

---

## 🔹 Results

* **Training Accuracy (KNN)** ≈ 100%
* **Validation Accuracy (KNN)** ≈ 34%
* **Random Classifier Accuracy** ≈ 16%

---

## 🔹 Observations

* KNN performs better than random classifier
* 1-NN overfits training data
* Validation accuracy is lower because data is unseen
* Accuracy improves slightly with multiple splits

---

## 🔹 Answers to Questions

### 1. Effect of validation size

Increasing validation size reduces training data and decreases accuracy, while decreasing validation size improves accuracy.

---

### 2. Effect of dataset size

Larger validation sets give more reliable results, while smaller ones lead to unstable accuracy.

---

### 3. Best split ratio

A good split is 70-30 or 80-20 for balanced performance.

---

### 4. Cross-validation

Averaging accuracy over multiple splits gives more stable and accurate results.

---

### 5. 1-NN vs 3-NN

* 1-NN → overfits, unstable
* 3-NN → more stable, better generalization

---

## 🔹 Conclusion

This lab demonstrates the importance of model evaluation in machine learning. The KNN model performs better than random classification but suffers from overfitting. Cross-validation improves reliability, and choosing appropriate parameters like K and data split significantly affects performance.

---

## 🔹 Key Learnings

* Difference between classification and regression
* Importance of evaluation metrics
* Role of train-test split
* Concept of overfitting
* Importance of cross-validation

---

