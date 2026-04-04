# Lab 03 – Data Augmentation

## Overview

This lab focuses on **Data Augmentation**, a technique used to increase the size of a dataset by creating modified versions of existing data. This helps improve machine learning model performance, especially when the dataset is small.

We use the **MNIST dataset** and apply transformations like rotation and shear.


## Objectives

* Understand data augmentation
* Apply transformations to images
* Increase dataset size artificially
* Improve model accuracy
* Analyze augmentation impact


##  Key Concepts

###  Data Augmentation

Creating new data from existing data using transformations.

###  Important Rule

Augmentations must preserve labels.

Rotate “3” → still “3”
Flip “6” → becomes “9”



##  Techniques Used

### 1. Rotation

* Rotating images by small angles
* Helps model handle different orientations

### 2. Shear

* Slants the image
* Adds variation in shape

### 3. Combination

* Rotation + Shear together



##  Results

* Baseline Accuracy: ~64–65%
* After Augmentation: ~67–68%
* Improvement: ~3%



## Observations

* Small transformations improve accuracy
* Large transformations reduce performance
* Rotation works better than shear
* Combining augmentations not always helpful



##  Questions & Answers

### Q1: Best parameters?

Angle ≈ 30°, Shear ≈ 0.8



### Q2: More augmentation helps?

Yes initially, but too much causes confusion



### Q3: Other augmentations

* Translation
* Scaling
* Noise addition



### Q4: Combining methods

Rotation alone worked best in this lab



##  Conclusion

Data augmentation improves model generalization and increases accuracy without collecting new data.



##  Key Takeaway

More meaningful data → Better model performance
