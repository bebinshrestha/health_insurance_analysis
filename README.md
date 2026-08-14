## **Health Insurance Cost Analysis** 

## Overview  
This data contains clean and structured insurance data including demographic information, risk factor, smoking status,insurance tier, and insurance charges. The primary objective of this project is to analyze the factors that influence health insurance cossts and understand how variables such as age, BMI, and smoking habits contribute to overall insurance charges. 

## Data Sources
 1. Source: kaggle.com
 Medical Insurance Charges (2021-2025) Enhanced
 Link: https://www.kaggle.com/datasets/ibrahimshahrukh/medical-insurance-cost-dataset-usa/data
 2. Source: kaggle.com
 Health Insurance Cost and Risk
 Link: https://www.kaggle.com/datasets/mjawad17/health-insurance-cost-and-risk-dataset
 
## Repository Contents
- medical_insurance_2026_kaggle.csv - dataset containing multiple years of insurance charges based on age, insurance tier, and risk factor. 
- health_insurance_cost_and_risk_dataset.csv - dataset containing insurance charges based on age, risk factor and annual income
- Health_Insurance_Analysis.ipynb - Jupyter Notebook 
- requirements.txt
- README.md
- ERD Diagram

## Project Objectives
- Analyze the relationship between insurance charges and demographic factor  
- Identify major contributor to higher insurance costs
- Visulizations

## Analysis and Visulization     
  - Data cleaing and wrangling    
  - Exploratory Data Analaysis (EDA)  
  - Impact of age on insurance charges (scatter plot)
  - Smoking status impact on insurance charges (scatter plot)
  - Age distribution and impact of age on insurance charges (histogram)
  - Average insurance charges based by region and smoking status (bar plot)


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

3. #### Create, Activate, and Deactivate Virtual Environment
```bash
python -m venv venv
source venv/Scrips/activate
deactivate
```

4. #### Install Dependencies
```bash 
pip install -r requirements.txt
```

5. #### Create Database File
The SQLlite database(../Data/Health_insurance.db) is not included in this repository because of the file size limit.
The database can be created using the following python code:
```python
conn = sqlite3.connect('../Data/health_insurance.db')
conn.execute("PRAGMA foreign_keys = ON")
regions_df.to_sql('regions', conn, if_exists = 'replace', index=False)
demographic_df.to_sql('demographic', conn, if_exists = 'replace', index=False)
policy_df.to_sql('policy', conn, if_exists = 'replace', index=False)
health_profile_df.to_sql('health_profile', conn, if_exists = 'replace', index=False)
```


## Findings
This analysis identified several patterns in health insurance charges:
- Insurance charges generally increases with age.
- Smokers has substantially higher average insurance charges than non-smokers across every region.
- Overall, smoking status is one of the strongest factor associated with higher insurance charges

## Author
Bebin Shrestha - Code:You Student

## AI Assistance
ChatGPT was used to review and troubleshoot the code when coding error arose and clarify the functions of the codes when needed. 


## License
Open source under the Creative Commons which states that "you can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission." 