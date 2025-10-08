# DataFun-07-ML  
**Author:** Brendon McNulty  

---

## 🎯 Project Overview

This project explores **Machine Learning with Linear Regression** using real NYC weather data.  
We apply a complete machine learning workflow — from data acquisition to prediction — to model and forecast **average January high temperatures** in New York City.

The project is divided into three main parts, progressively building skills in data handling, modeling, and visualization.

---

## 🧱 Part 1 — Chart a Straight Line (10.16)

We began by revisiting the equation for a straight line:

\[
F = \frac{9}{5}C + 32
\]

- Practiced plotting a perfect linear model between **Celsius and Fahrenheit** using Matplotlib.  
- Explored the meaning of slope (*m*) and intercept (*b*) in a simple, exact linear relationship.  
- Visualized the relationship where each Celsius value maps perfectly to Fahrenheit — demonstrating a **perfect linear correlation**.

---

## 🌡️ Part 2 — Predict NYC January High Temperatures

We transitioned from theoretical data to **real-world data** — NYC’s January high temperatures from **1895–2018**.

Steps included:
1. **Data Acquisition:** Loaded the dataset into a Pandas DataFrame.  
2. **Data Inspection:** Reviewed structure and content with `.head()` and `.tail()`.  
3. **Data Cleaning:** Renamed columns, handled missing values, and ensured date accuracy.  
4. **Descriptive Statistics:** Used `.describe()` to summarize central tendency and spread.  

We then used **SciPy’s `linregress()`** to calculate:
- Slope (*m*) — the rate of change in temperature over time.  
- Intercept (*b*) — the base temperature where the regression line crosses the y-axis.  

Our fitted line took the form:

\[
\hat{y} = m \cdot x + b
\]

where  
- \( \hat{y} \) = predicted temperature  
- \( x \) = year  
- \( m \) = slope  
- \( b \) = intercept  

---

## 📈 Part 3 — Build, Test, and Predict

In the final stage, we:
1. **Built and tested** the model using `train_test_split` for training and validation.  
2. **Predicted** the **average NYC January high temperature for 2024**.  
3. **Visualized** the regression model using Seaborn and Matplotlib with a best-fit line overlayed on the scatter plot of historical data.

The model revealed a **gradual upward trend** in average January temperatures over more than a century, consistent with long-term climate warming trends.

---

## Final Analysis and Reflection

This project demonstrated how linear regression can model real-world data trends while introducing the fundamental workflow of **supervised learning**.

Key takeaways:
- Linear regression can effectively model continuous numeric trends over time.  
- Historical climate data provides an excellent example of linear relationships with real impact.  
- Visualization helps connect mathematical models with intuitive understanding.  

Although the linear model captures general warming, more advanced models (like polynomial regression or time series forecasting) could provide deeper insight into non-linear or seasonal climate effects.

---

## Tools and Technologies
- **Python**
- **JupyterLab**
- **NumPy**, **Pandas**, **SciPy**, **Matplotlib**, **Seaborn**
- **Scikit-learn** (for model training and testing)
- **Git & GitHub** for version control

---

## How to Run This Project

1. Clone the repository  
   ```bash
   git clone https://github.com/YOUR_USERNAME/datafun-07-ml.git
   cd datafun-07-ml


---

##  Project Structure
datafun-07-ml/
│
├── examples/
│ └── ch15/
│ ├── ave_hi_nyc_jan_1895-2018.csv
│
├── brendon_ml_final.ipynb # Final machine learning project notebook
├── README.md # Project overview and reflection
└── requirements.txt # Dependencies