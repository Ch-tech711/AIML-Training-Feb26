# 📊 Module 2: Appreciating, Interpreting and Visualizing Data

## 🧪 Lab 1: Basic Plots using Matplotlib & Seaborn

---

## 🎯 Aim

To understand and visualize the automobile dataset using various plotting techniques such as Scatter Plot, Box Plot, Violin Plot, Swarm Plot, and Joint Plot.

---

## 🛠 Tools & Libraries Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn

---

## 📂 Dataset

* Automobile Dataset (1985 Ward’s Automotive Yearbook)
* Contains features like:

  * Car maker
  * Price
  * Horsepower
  * Mileage
  * Body style

---

## 🔄 Steps Performed

### 1. Data Loading

* Imported dataset from URL using `requests`
* Converted into Pandas DataFrame

### 2. Data Cleaning

* Replaced missing values (`"?"`) with `NaN`
* Removed rows with missing data

### 3. Feature & Target Separation

* Features (X): All columns except price
* Target (y): Price column

---

## 📊 Visualizations & Observations

### 🔹 Scatter Plot (Make vs Price)

* Shows relationship between car manufacturer and price
* High-end brands like Mercedes-Benz, Jaguar, Porsche have higher prices

---

### 🔹 Box Plot (Make vs Price)

* Displays median, spread, and outliers
* Mercedes-Benz and Jaguar have highest median prices
* BMW shows wide variation in prices

---

### 🔹 Violin Plot (Make vs Price)

* Shows distribution and density of prices
* Wider sections indicate higher data concentration
* Helps understand how prices are spread within each brand

---

### 🔹 Swarm Plot

* Displays individual data points clearly
* Avoids overlapping of points
* Useful for smaller datasets

---

### 🔹 Box Plot (Make vs Horsepower)

* Shows horsepower distribution across brands
* Sports brands like Porsche and Jaguar have higher horsepower

---

### 🔹 Scatter Plot (Horsepower vs Price)

* Shows **positive correlation**
* As horsepower increases, price also increases

---

### 🔹 Joint Plot

* Combines scatter plot with regression line and distributions
* Clearly shows relationship between variables

---

### 🔹 Joint Plot (Highway-mpg vs Price)

* Shows **negative correlation**
* Higher mileage cars tend to have lower prices

---

### 🔹 Box Plot (Body Style vs Price)

* Convertible has highest median price
* Hatchback has lowest price range
* Body style affects car price significantly

---

## 📌 Task Performed

* Plotted **Box Plot and Violin Plot together** using subplots
* Used an additional plot type (**Strip Plot**) to visualize individual data points

---

## 🧠 Key Concepts Learned

* Data Visualization techniques
* Understanding distributions and density
* Identifying outliers
* Correlation (positive & negative)
* Comparing categorical data

---

## ✅ Conclusion

Data visualization helps in understanding patterns, relationships, and trends in data effectively.
Different plots provide different insights:

* Scatter Plot → Relationship
* Box Plot → Summary & Outliers
* Violin Plot → Distribution
* Joint Plot → Correlation

These visual tools make it easier to analyze and interpret complex datasets.

---

## 🚀 Outcome

Successfully visualized and interpreted the automobile dataset using multiple plotting techniques.

---


# 📘 AIML Module 2 – Lab 2  
## 📊 Principal Component Analysis (PCA)

---

## 📌 Overview
This lab focuses on **Principal Component Analysis (PCA)**, a widely used **linear dimensionality reduction** technique. PCA transforms high-dimensional data into a lower-dimensional space while preserving as much variance as possible.

---

## 🎯 Objectives
- Understand the concept of dimensionality reduction  
- Learn how PCA works mathematically  
- Implement PCA manually  
- Apply PCA using Scikit-learn  
- Visualize high-dimensional data in lower dimensions  

---

## 🧩 What is PCA?
PCA (Principal Component Analysis) is a technique that:
- Reduces the number of features  
- Preserves maximum variance  
- Converts correlated variables into uncorrelated principal components  

---

## ⚙️ Algorithm Steps
1. Standardize the dataset  
2. Compute covariance matrix  
3. Calculate eigenvalues and eigenvectors  
4. Sort eigenvalues in descending order  
5. Select top k eigenvectors  
6. Transform data into new feature space  

---

## 🧪 Experiments

### 1. Data Standardization
- Center the data (mean = 0)  
- Scale features if required  

### 2. Covariance Matrix
- Measures relationship between features  

### 3. Eigenvalues & Eigenvectors
- Eigenvectors → directions of maximum variance  
- Eigenvalues → magnitude of variance  

### 4. Dimensionality Reduction
- Select top components  
- Project data onto new axes  

### 5. Visualization
- Plot reduced data in 2D or 3D  

---

## 📊 Observations
- PCA reduces dimensionality effectively  
- Helps remove redundancy in data  
- Works well for linear datasets  
- May not perform well for non-linear data  

---

## 🛠️ Technologies Used
- Python  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## 📁 Files
- AIML_Module_2_Lab2_Principal_Components_Analysis_(PCA).ipynb  
- README.md  

---

## 🚀 How to Run
1. Install dependencies:
   pip install numpy matplotlib scikit-learn  

2. Open Jupyter Notebook:
   jupyter notebook  

3. Run all cells  

---

## 📚 Learning Outcomes
- Understanding PCA concepts  
- Ability to reduce dimensions of data  
- Knowledge of eigenvalues and eigenvectors  
- Practical implementation using Python  

---

## ✍️ Conclusion
PCA is a powerful and efficient technique for reducing dimensionality in datasets. It simplifies data while retaining important information, making it useful for visualization, noise reduction, and preprocessing in machine learning.


# 📘 AIML Module 2 – Lab 3  
## 🧠 Manifold Learning using Isomap

---

## 📌 Overview
This lab focuses on **Manifold Learning**, a non-linear dimensionality reduction technique. We implement and understand the **Isomap algorithm**, which preserves the intrinsic geometry of data lying on a curved manifold.

---

## 🎯 Objectives
- Understand manifolds in machine learning  
- Learn how Isomap works  
- Implement Isomap manually  
- Use Scikit-learn’s Isomap  
- Apply on synthetic and real datasets  

---

## 🧩 What is Isomap?
Isomap (Isometric Mapping) is a non-linear dimensionality reduction technique that preserves **geodesic distances** instead of Euclidean distances.

---

## ⚙️ Algorithm Steps
1. Build neighborhood graph using k-nearest neighbors  
2. Compute geodesic distances using shortest path algorithm  
3. Apply eigen decomposition for dimensionality reduction  

---

## 🧪 Experiments

### 1. Synthetic Dataset (S-Curve)
- Generated using `make_s_curve()`  
- Goal: Reduce 3D data into 2D while preserving structure  

### 2. Manual Implementation
- Distance matrix computation  
- Graph construction  
- Shortest path calculation  
- Eigen decomposition  

### 3. Scikit-learn Isomap
- Efficient built-in implementation  
- Easy to apply on datasets  

### 4. Face Dataset
- High-dimensional image data  
- Compared Isomap with PCA  
- Isomap preserves structure better  

---

## 📊 Observations
- Isomap works well for non-linear data  
- Preserves global structure  
- Performs better than PCA for curved datasets  

---

## 🛠️ Technologies Used
- Python  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## 📁 Files
- AIML_Module_2_Lab_3_Manifold_Learning_Methods.ipynb  
- README.md  

---

## 🚀 How to Run
1. Install dependencies:
   pip install numpy matplotlib scikit-learn  

2. Open Jupyter Notebook:
   jupyter notebook  

3. Run all cells  

---

## 📚 Learning Outcomes
- Understanding of manifold learning  
- Difference between linear and non-linear methods  
- Hands-on with Isomap implementation  

---

## ✍️ Conclusion
Isomap is an effective method for dimensionality reduction when dealing with non-linear data structures, making it useful in visualization and real-world machine learning tasks.
