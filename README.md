# Mortality

## Table of Contents

- [Project Overview](#project-overview)
- [Tools](#tools)
- [Data Analysis](#data-analysis)
- [Recommendations](#recommendations)

### Project Overview

This project explores the analysis of mortality rates between 1970 and 2010. Our objective is to identify patterns, provide evidence-based recommendations, and attain an in-depth understanding of mortality by examining various aspects. This involves investigating factors such as the age group with the highest number of deaths, countries with dominance in mortality, which gender leads in mortality, and the trend of mortality.

<img width="776" alt="Mortality dashboard picture" src="https://github.com/IanLiam/Mortality_Dashboard-Tableau-/assets/117744677/fff64007-aff2-4863-afe9-ebfc6368eb60">

### Data Sources
The dataset utilized for this analysis is the "Mortality.csv" file, which comprises comprehensive details.

### Tools
- Excel - Data Cleaning  [Download here](https://www.microsoft.com/en-us/microsoft-365/download-office)
- Python - Data Cleaning  [Download here](https://www.anaconda.com/download)
- SQL Server - Data Analysis [Download here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- Tableau - Creating reports  [Download here](https://www.tableau.com/community/public)
  
### Data cleaning/ Preparation
In the initial data preparation phase, we performed the following tasks:

1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

### Exploratory Data Analysis
EDA involved exploring the Mortality data to answer key questions, such as:

- Which gender leads in mortality rates?
- Which country has the highest number of deaths?
- Which age group dominates in mortality?

### Data Analysis
Features worked with:

1. SQL
```sql
-- Selecting with a condition
SELECT * FROM Mortality
where gender = 'Male';
```

2. Python
```python
# Transposing data
import pandas as pd

# Replace 'input.csv' with the path to your CSV file
input_file = r'C:\Users\ian.muthengi\Downloads\Mortality.xlsx'

# Read the CSV file into a pandas DataFrame
df = pd.read_excel(input_file)

# Transpose the DataFrame
df_transposed = df.transpose()

# Replace 'output_transposed.csv' with the desired output file name
output_file = 'C:/Users/ian.muthengi/Downloads/transposed_Mortality.xlsx'

# Write the transposed DataFrame to a new CSV file
df_transposed.to_excel(output_file, index=True, header=False)
```
### Results/Findings
The analysis results are summarized as follows:

1. The male gender dominates in mortality, with a total of 127,970,255 cases.
2. India has the highest number of deaths at 47,019,810.
3. The 80+ age group leads in mortality.

### Recommendations
Based on the analysis, we recommend the following actions:

1. Ensure that individuals, especially those in vulnerable age groups like the elderly, have access to quality healthcare services.
2. Encourage and promote a healthy lifestyle among all age groups.
3. Increase public awareness and education about factors that contribute to mortality.

### Limitations
Incomplete data
