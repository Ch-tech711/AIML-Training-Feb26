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
