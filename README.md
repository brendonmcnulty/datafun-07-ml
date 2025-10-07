# Machine Learning Final Project  
**Author:** Brendon McNulty  

---

## 🎯 Project Overview
This project demonstrates the foundational concepts of **machine learning** through two linear modeling exercises:  
1. A simple mathematical example illustrating a **perfect linear relationship** (Celsius → Fahrenheit).  
2. A real-world **regression analysis** predicting average January high temperatures in New York City using historical data from 1895–2018.

The notebook, **`brendon_ml_final.ipynb`**, walks through every step of the professional data workflow — from loading and inspecting data to modeling, prediction, and visualization with confidence intervals.

---

## 🧩 Tools and Libraries
The following libraries were used:
- **pandas** — data manipulation and cleaning  
- **NumPy** — numeric computation  
- **matplotlib / seaborn** — data visualization  
- **SciPy** — regression modeling (`stats.linregress`)  
- **scikit-learn** — data splitting and potential model comparisons  

---

## 🧮 Part 1 — Chart a Straight Line (Celsius to Fahrenheit)
To introduce linear relationships, a simple function was created to convert Celsius to Fahrenheit:

\[
F = \frac{9}{5}C + 32
\]

Using a **lambda function** and **list comprehension**, a set of temperature pairs was generated and displayed as a labeled DataFrame.  
A corresponding plot was created to visualize this perfect linear relationship.

**Key takeaway:**  
Every Celsius–Fahrenheit pair lies exactly on the same line, showing a **perfect linear correlation** — an ideal foundation for understanding linear regression.

---

## 🌡️ Part 2 — Predicting NYC January High Temperatures (1895–2018)

### **Sections 1–4: Data Preparation**
- Loaded data from `ave_hi_nyc_jan_1895-2018.csv`
- Inspected the dataset (`head()`, `tail()`, `info()`)
- Cleaned and renamed columns (`Year`, `Temperature`, `Anomaly`)
- Extracted `Year` from the combined `Date` column
- Generated descriptive statistics and visualized temperature trends over time

**Observation:**  
The raw data shows natural year-to-year variability with a gradual upward trend, suggesting long-term warming.

---

### **Sections 5–7: Linear Regression Model, Prediction, and Visualization**
Used **SciPy’s `linregress`** to compute the best-fit line:

\[
\hat{y} = m x + b
\]

**Model outputs included:**
- Slope (`m`)
- Intercept (`b`)
- Correlation coefficient (`r`)
- P-value
- Standard error of slope

**Prediction:**  
The model was then used to estimate the **average January high temperature for 2024**.

**Visualization:**
- Scatter plot of historical data (Year vs. Temperature)
- Best-fit regression line overlay
- Highlighted 2024 predicted value in red
- Added **95% confidence interval shading** to show the model’s uncertainty range

**Result:**  
The regression line reveals a gradual upward trend over time, consistent with observed warming patterns in NYC’s winter climate.

---

## 🧠 Key Learnings and Takeaways
- Learned how to implement **linear regression** using both mathematical logic and real data.
- Understood how to interpret slope, intercept, and correlation statistics.
- Practiced **data cleaning**, **feature extraction**, and **visual storytelling** using Python.
- Added **confidence intervals** to communicate model reliability visually.
- Combined both **perfect and imperfect** examples to understand how real-world data differs from theoretical relationships.

---

## 🗂️ Project Structure
datafun-07-ml/
│
├── examples/
│ └── ch15/
│ ├── ave_hi_nyc_jan_1895-2018.csv
│
├── brendon_ml_final.ipynb # Final machine learning project notebook
├── README.md # Project overview and reflection
└── requirements.txt # Dependencies