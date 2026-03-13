# Lab 03 – Probability & Statistics for Machine Learning

 Overview

This lab introduces important **probability distributions and statistical concepts** that are widely used in Machine Learning and Data Science.
It focuses on modeling randomness, understanding distributions, and exploring how uncertainty is quantified in data.

The notebook demonstrates both **theoretical concepts and Python implementations** using scientific computing libraries.

---> Topics Covered

1. Binomial Distribution

The binomial distribution models the probability of obtaining a fixed number of successes in a fixed number of independent trials.

Examples:

* Coin toss experiments
* Success/failure outcomes

Functions used:

* `binom.pmf()`
* `binom.cdf()`

2. Normal Distribution

The normal distribution (Gaussian distribution) is a continuous probability distribution characterized by a bell-shaped curve.

Key parameters:

* Mean (μ)
* Standard Deviation (σ)

Functions used:

* `norm.pdf()` – Probability Density Function
* `norm.cdf()` – Cumulative Distribution Function
* `norm.ppf()` – Percent Point Function (inverse CDF)

3. Empirical Rule (68–95–99.7 Rule)

For normally distributed data:

* 68% of values lie within **1 standard deviation**
* 95% lie within **2 standard deviations**
* 99.7% lie within **3 standard deviations**

This rule helps quickly estimate probabilities in a normal distribution.

 4. Poisson Distribution

The Poisson distribution models the probability of a number of events occurring in a fixed time interval.

Examples:

* Number of emergency calls per hour
* Number of website visits per minute

Function used:

* `poisson.pmf()`

 5. Central Limit Theorem (CLT)

The Central Limit Theorem states that the distribution of sample means approaches a **normal distribution** as the sample size increases, regardless of the original population distribution.

This theorem explains why the normal distribution appears frequently in statistics and machine learning.

6. Entropy (Information Theory)

Entropy measures the **uncertainty or randomness** in a system.

Formula:

H(X) = − Σ P(x) log₂ P(x)

Higher entropy → more unpredictability
Lower entropy → more predictable outcomes

Applications:

* Decision Trees
* Information Gain
* Data Compression

 7. Huffman Coding

Huffman coding is a **lossless data compression algorithm** that assigns shorter binary codes to more frequent symbols and longer codes to less frequent symbols.

Applications:

* File compression (ZIP)
* Image compression
* Data storage optimization
  
---> Libraries Used

* NumPy
* SciPy
* Matplotlib
* Seaborn

## Notebook

The implementation and experiments for this lab are available in:

`AIML_Course_Probability_Primer.ipynb`

## Learning Outcomes

After completing this lab, we understand:

* How probability distributions model real-world randomness
* The importance of the normal distribution in statistics
* The role of the Central Limit Theorem in data analysis
* How entropy measures uncertainty in information systems
* How Huffman coding enables efficient data compression
