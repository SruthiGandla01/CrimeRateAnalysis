# 🕵️‍♀️ ARIMA-Based-Crime-Forecasting

This project performs a comprehensive analysis of crime data from 2020 to the present. Using Python, data visualization tools, and ARIMA-based time series forecasting, it uncovers patterns in criminal activity and predicts future crime rates. The goal is to enable proactive planning, risk assessment, and public safety strategy formulation.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Procedure](#procedure)
- [Features](#features)
- [Data Sources](#data-sources)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Conclusion](#conclusion)

---

## 📊 Project Overview

The Crime Rate Analysis project explores crime trends using structured exploratory data analysis (EDA) and forecasting techniques. It identifies patterns across time, geography, and offense types and uses the ARIMA model to project future crime levels. This combination of retrospective and predictive insights is valuable for policy makers, law enforcement, and researchers.

---

## 🔍 Procedure

This project follows a structured approach to explore, clean, analyze, and forecast crime data. The major steps are outlined below:

### 1. Data Acquisition

The crime dat is loaded using `pandas` from a CSV file titled `Crime_Data_from_2020_to_Present.csv`. It contains fields such as `Date Reported`, `Area Name`, and `Crime Description`.

```python
import pandas as pd
crime_data = pd.read_csv('Crime_Data_from_2020_to_Present.csv')
```


### 2. Data Inspection
Initial inspection includes:

Checking data types and completeness using .info()

Previewing data with .head()

Identifying inconsistencies or unexpected values

### 3. Data Cleaning
Steps performed:

Removing missing or null values in critical columns like date or area

Renaming columns for clarity

Filtering out redundant or irrelevant data

Standardizing date formats and textual labels

### 4. Feature Selection & Transformation
From the full dataset, only essential features are selected:

DATE REPORTED

AREA NAME

CRIME CODE DESC

Transformations include:

Converting date fields to datetime type

Extracting month and year

Grouping crimes by time period (monthly) for trend analysis

### 5. Exploratory Data Analysis (EDA)
Visualizations include:

Total crimes per year

Top 10 most common crime categories

Area-wise crime counts

Monthly crime trends

These insights are plotted using matplotlib and seaborn, offering a clear understanding of spatial and temporal crime distributions.

### 6. Time Series Forecasting using ARIMA
To anticipate future crime levels:

Monthly crime totals are calculated

An ARIMA(1,1,1) model is trained on the time series

The model forecasts the number of crimes for the next 12 months

Confidence intervals and trends are plotted for interpretability

This helps predict upcoming surges and better allocate law enforcement resources.

### 7. Reporting
All results are documented in a comprehensive PDF report, covering:

The methodology used

EDA findings

Forecast interpretation

Visualizations

Recommendations for future work

### 🚀 Features
📊 In-depth EDA with plots for annual and monthly trends

🔍 Area-wise and category-wise crime breakdown

📈 Forecasting future crime rates using ARIMA

📄 Structured and clean reporting of key insights

### 📂 Data Sources
Dataset: Crime_Data_from_2020_to_Present.csv

Includes:

Crime description and classification

Area and location information

Date reported

Crime resolution status

### 🛠️ Technologies Used
**Lan: Python

Libraries: Pandas, Matplotlib, Seaborn, Statsmodels

Notebook Tool: Jupyter Notebook

### ✅ Conclusion

This project demonstrates how data science can enhance public safety through crime analysis and forecasting. combining EDA with time series modeling, it empowers stakeholders to understand current crime dynamics and prepare for the future. The insights and tools developed here can support better policies, law enforcement strategies, and public awareness efforts.
