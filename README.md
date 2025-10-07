# DataFun-07-ML  
**Author:** Brendon McNulty  

---

## Module Goal  
In this module, we begin a guided machine learning project. We create and manage a professional workflow using GitHub for version control, VS Code for development, and JupyterLab for exploration and analysis.  

We'll use predictive analytics and introduce machine learning concepts while following a repeatable, professional data workflow.  

---

## Project Setup Steps  

### 1. Create and Clone the Repository  
Created a new GitHub repository named **datafun-07-ml** with a default `README.md`.  
Cloned the repository to the local folder:  

git clone https://github.com/your-username/datafun-07-ml.git
cd datafun-07-ml

yaml
Copy code

---

### 2. Add Common Project Files  
Added `.gitignore` and `requirements.txt` to define dependencies and ignored files.  

**.gitignore includes:**  
.venv/
pycache/
.ipynb_checkpoints/
.vscode/
data/

markdown
Copy code

**requirements.txt includes:**  
jupyterlab
numpy
pandas
pyarrow
matplotlib
seaborn
scipy
scikit-learn

yaml
Copy code

---

### 3. Create and Activate Virtual Environment  
Created and activated a virtual environment to isolate dependencies:  

py -m venv .venv
.venv\Scripts\Activate
py -m pip install --upgrade pip
py -m pip install -r requirements.txt

yaml
Copy code

---

### 4. Launch JupyterLab  
Launched JupyterLab to begin analysis and machine learning exploration:  

jupyter lab

yaml
Copy code

---

## Chapter 10: Object-Oriented Programming (OOP)  
In this section, we reviewed object-oriented programming concepts using Python classes and methods.  

### Example: Custom `Account` Class  
We imported and ran an example from the Deitel & Associates textbook repository to explore:  
- How Python uses classes and objects  
- How attributes (data) and methods (functions) interact inside a class  

We created an instance of the `Account` class, deposited funds, and printed a formatted balance message.  

**Key Concepts:**  
- Encapsulation and data protection using attributes  
- Methods for interacting with data (e.g., `deposit()`, `withdraw()`)  
- Using class instances to represent real-world entities  

---

## Chapter 15: Machine Learning Examples  

### Example 1 — Time Series & Simple Linear Regression (`15_04.py`)  
This example uses **pandas** and **scikit-learn** to model NYC January temperature trends from 1895–2018.  

**Key Steps:**  
- Load data from `ave_hi_nyc_jan_1895-2018.csv`  
- Train and test a **Linear Regression** model  
- Predict future and past temperatures  
- Visualize the regression trendline with **Seaborn** and **Matplotlib**  

**Result:**  
A regression line showing a gradual increase in average NYC January temperatures over time.  

---

### Example 2 — Dimensionality Reduction with t-SNE (`15_06.py`)  
This example demonstrates **unsupervised learning** using t-SNE to reduce high-dimensional data (handwritten digits) into a 2D representation.  

**Key Steps:**  
- Load digit data from `sklearn.datasets.load_digits()`  
- Apply **t-SNE** (`sklearn.manifold.TSNE`) for dimensionality reduction  
- Visualize the clusters in 2D with **Matplotlib**  

**Result:**  
Each cluster corresponds to a digit (0–9), showing how t-SNE groups similar features together visually.  

---

## Skills and Concepts Covered  
- Object-Oriented Programming  
- Data exploration with pandas  
- Train-test splitting with scikit-learn  
- Linear Regression modeling  
- Data visualization with Seaborn and Matplotlib  
- Dimensionality reduction (t-SNE)  
- Version control with Git & GitHub  
- Reproducible data workflows  

---

## Summary  
This module combined object-oriented principles with foundational machine learning workflows.  
Through both supervised and unsupervised examples, we practiced real-world data handling, model training, and visualization techniques using professional tools like **JupyterLab**, **VS Code**, and **GitHub**.  

---

## Repository Structure  
datafun-07-ml/
│
├── .venv/ # Virtual environment (ignored by Git)
├── examples/
│ └── ch15/
│ ├── 15_04.py # Time Series Linear Regression
│ ├── 15_06.py # t-SNE Dimensionality Reduction
│ └── ave_hi_nyc_jan_1895-2018.csv
│
├── ml_ch10_intro.ipynb # OOP examples and explanations
├── ml_ch15_examples.ipynb # Machine Learning examples and visualizations
├── README.md # Project overview and documentation
└── requirements.txt # Dependencies list