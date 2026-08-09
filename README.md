## **Medical Insurance Charges** 

## Overview  
This data contains clean and structured insurance data including demographic information, risk factor, smoking status,insurance tier, and insurance charges. The primary objective of this project is to analyze the factors that influence health insurance cossts and understand how variables such as age, BMI, and smoking habits contribute to overall insurance charges. 
 
## Repository Contents
- medical_insurance_2026_kaggle.csv - dataset containing multiple years of insurance charges based on age, insurance tier, and risk factor. 
- health_insurance_cost_and_risk_dataset.csv - dataset containing insurance charges based on age, risk factor and annual income
- Health_Insurance_Analysis.ipynb - Jupyter Notebook 
- requirements.txt
- README.md

## Project Objectives
- Analyze the relationship between insurance charges and demographic factor  
- Identify major contributor to higher insurance costs
- Visulizations

## Analysis and Visulization     
  - Data cleaing and wrangling    
  - Exploratory Data Analaysis (EDA)  
  - 
  - Distribution of gender and insurance charges by gender (pie chart and bar plot)
  - Age distribution and impact of age on insurance charges (histogram and scatter plot)
  - Smoking status impact on insurance charges (scatter plot)
  - Correlation analysis (Head Map)
  - Impact of BMI and smoking status on insurance charges (bar plot)

## Instructions
1. #### Fork and Clone the Repository
```bash
   git clone https://github.com/bebinshrestha/health_insurance_analysis.git
```
2. #### Open the Notebook
   Open 'Health_Insurance_Analysis.ipynb' in Jupyter Notebook
## Usages
```bash
import pandas as pd 
import matplotlib.pyplot as plt 
import numpy as np 
import seaborn as sns 
import sqlite3
```
```bash
df = pd.read_csv("data/medical_insurance_2026_kaggle.csv")
df.head()
df1 = pd.read_csv("../data/health_insurance_cost_and_risk_dataset.csv")
df1.head()
```

## Author
Bebin Shrestha - Code:You Student

## License
Open source under the Creative Commons which states that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission." 