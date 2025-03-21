# 🚗 AI-Based Car Insurance Claims Analysis

This project presents a structured approach to analyzing car insurance claim datasets using **Exploratory Data Analysis (EDA)** and **statistical techniques**. It aims to extract valuable insights, uncover patterns, and prepare data for further modeling.

<center><img alt="Insight logo" src="https://raw.githubusercontent.com/warazkhan/CarInssurance-DataAnalysis/main/carInssuranceClaimGif.gif" align="center" hspace="10px" vspace="10px" width=80% height=100% ></center>

## 📌 Project Overview
- **Dataset**: Contains information about individual customers, their socio-demographic profiles, and vehicle details.
- **Objectives**:
  - Perform EDA to extract meaningful insights.
  - Understand the relationships between different variables.
  - Identify trends, correlations, and potential fraudulent claims.
  - Preprocess the dataset for machine learning models.

## 🔍 Key Analysis Techniques
### 📊 **Univariate Analysis**
- Examines a **single variable** at a time.
- Findings:
  - **Females** show a higher preference for insurance.
  - Most insured individuals are **married, have completed high school, use cars privately, and live in urban areas**.
  - A small percentage had their **licenses revoked**.

### 🔄 **Bivariate & Multivariate Analysis**
Bivariate and multivariate analyses explore relationships between two or more variables simultaneously, providing deeper insights.
  
1️⃣ **Categorical to Categorical Analysis**  
   - A **higher proportion of females** had their licenses revoked.
   - **Married individuals** with high school degrees formed a significant portion of policyholders.

2️⃣ **Numerical to Numerical Analysis**  
   - **Income** significantly affects **claim amounts** and **claim frequencies**.

3️⃣ **Categorical to Numerical Analysis**  
   - **PhD holders** tend to have higher **claim amounts**.
   - **Doctors** have higher **incomes**.
   - **Individuals above 73 years old** predominantly belong to **professional occupations**.

## 🛠️ Data Preprocessing Techniques
The dataset undergoes **cleaning, transformation, and feature engineering** before analysis.

1️⃣ **Frequency Plots (Histograms)**  
   - Visualize the distribution of variables.

2️⃣ **Discrete Statistics**  
   - **Measures of central tendency**: Mean, median, and mode.  
   - **Variability measures**: Range, standard deviation, and variance.  
   - **Skewness & Kurtosis** to assess distribution shape and concentration.

3️⃣ **Outlier Detection & Treatment**  
   - **Univariate outliers** identified using **Interquartile Range (IQR)**.  
   - **Multivariate outliers** replaced with the **mean** to prevent data loss.

4️⃣ **Handling Missing Values**  
   - **Numerical missing values**: Imputed with **mean or most frequent strategy**.  
   - **Categorical missing values**: Replaced with **most frequent category**.

5️⃣ **Correlation Analysis**  
   - Examines relationships between variables.  
   - **Positive & negative correlations** indicate strength & direction of relationships.  
   - Coefficients range from **-1 (perfect negative correlation) to 1 (perfect positive correlation)**.

6️⃣ **Normalization & Scaling**  
   - **Normalization** transforms data into a **normal distribution**.  
   - **Scaling (Min-Max, Z-score normalization)** ensures fair comparisons.

7️⃣ **Grouping Data**  
   - Segments data by **age, gender, driving record, and vehicle type**.  
   - Helps identify **patterns** and **trends** in different groups.

## 🔧 Tools & Libraries Used
This project utilizes the following Python libraries:
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
import plotly.graph_objects as go
from plotly.subplots import make_subplots
from scipy.stats import skew
from sklearn.impute import SimpleImputer
import warnings
warnings.filterwarnings('ignore')
