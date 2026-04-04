# AIML-Training-Feb26
IIIT Hyderabad AIML Training Program lab-1

AIML Module 01 - Lab 01: Feature Extraction from Data

This repository contains my lab work from the IIIT Hyderabad AIML Training Program.  
The objective of this lab is to explore "feature extraction" techniques from both "text data and image data".

# Part 1: Feature Extraction from Text
In this part, we worked with "Wikipedia" articles and extracted text features using "N-grams".

--> Tasks Performed
- Downloaded Wikipedia articles for "Giraffe" and "Elephant"
- Extracted "Unigrams (1-grams)"
- Extracted "Bigrams (2-grams)"
- Compared "bigram frequencies across different languages"
- Compared "bigram patterns for different topics"
- Visualized "Trigrams and higher n-grams"

--> Key Observations
- Bigram patterns are "similar across different topics" in the same language.
- Bigram patterns are "different across languages".
- Therefore,bigram frequency is useful for distinguishing languages but not topics.


# Part 2: Feature Extraction from Images

In this part, we worked with the "MNIST dataset", which contains handwritten digit images.
--> Dataset Information
- Each digit image has a size of "28 × 28 pixels"
- Each image is represented as a "784-dimensional vector"

--> Tasks Performed
- Loaded handwritten digit images
- Extracted simple features from the images
- Visualized and analyzed feature distributions
- Explored how features help distinguish between digits

-->  Technologies Used

- Python
- Google Colab
- NLTK
- Matplotlib
- Wikipedia API
- Scikit-learn
- MNIST Dataset

-->Conclusion

Feature extraction helps convert complex data such as "text and images into numerical features" that can be used for machine learning tasks.  
N-gram features are useful for analyzing text patterns, while pixel-based features help identify handwritten digits.
