## Indian Road Accident Analysis (2022–2025)
---
📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on Indian road accident data from 2022–2025. 
The goal is to identify accident patterns, severity trends, geographical hotspots, and factors that influence road accidents across India.
The analysis includes data cleaning, preprocessing, outlier detection, feature engineering, statistical exploration, and visualization.

---

📂 Dataset Features

The dataset contains information related to road accidents, including:

Date of Accident
State
City
Accident Severity
Weather Conditions
Road Type
Vehicles Involved
Casualties
Traffic Signal Information
Risk Score
Peak Hour Indicator

---

🛠 Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook

---

📊 Analysis Workflow
1. Data Loading
The dataset is loaded using Pandas.

df = pd.read_csv('Indian Road Accident (2022–2025) EDA.csv')

---
2. Data Inspection

Basic dataset exploration:

View top and bottom records
Check dataset shape
Inspect data types
Identify missing values
Detect duplicate records

---
3. Data Preprocessing
Date Conversion

df['date'] = pd.to_datetime(df['date'], format="%d-%m-%Y")

Feature Engineering
Additional date-based features are extracted:
Year
Month Name
Day Name

df['Year'] = df['date'].dt.year
df['Month_Name'] = df['date'].dt.month_name()
df['Day_Name'] = df['date'].dt.day_name()













