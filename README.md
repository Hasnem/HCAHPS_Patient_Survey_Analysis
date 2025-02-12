# HCAHPS Patient Satisfaction Analysis (2014–2023)

This repository explores Hospital Consumer Assessment of Healthcare Providers and Systems (**HCAHPS**) patient satisfaction data across U.S. hospitals from **2014 to 2023**.

---

## Table of Contents
1. [Overview](#overview)  
2. [Data Sources](#data-sources)  
3. [Project Workflow](#project-workflow)  
4. [Key Features](#key-features)  
5. [Technologies](#technologies)  
6. [Use Cases](#use-cases)  

---

<a id="overview"></a>
## 1. Overview

This analysis examines **HCAHPS (Hospital Consumer Assessment of Healthcare Providers and Systems)** patient satisfaction data from **2014 to 2023**. 

- **Purpose**: Identify trends in patient satisfaction, uncover pandemic impacts, and determine the strongest predictors of hospital ratings.  
- **Key Findings**:  
  - **Care Transition**, **Quietness**, and **Cleanliness** most strongly influence the Overall Hospital Rating.  
  - **Communication about Medicines** consistently underperforms, especially during COVID-19.  
  - Average Top-box scores dipped by ~2–3% during 2021–2022, but began recovering in 2023.

You can also explore an **interactive dashboard** showcasing these insights and trends, and check out the **source code** for deeper analysis.

---

<a id="data-sources"></a>
## 2. Data Sources
1. **Maven Analytics Data Playground**  
   - National & state-level HCAHPS data from 2013 to 2022.

2. **CMS HCAHPS (Hospital Compare) Archives**  
   - The last available date (2023) used to update the Maven dataset.

**Data Processing**:  
- All data was merged in `data_processor.ipynb` to create a final comprehensive dataset (2013–2023).

---

<a id="project-workflow"></a>
## 3. Project Workflow

1. **Data Merging**:  
   - `data_processor.ipynb` merges 2013–2022 data from Maven Analytics with 2023 CMS HCAHPS data.

2. **Exploratory Data Analysis (EDA)**:  
   - Identified trends in Top-box, Middle-box, and Bottom-box distributions.  
   - Analyzed how COVID-19 impacted specific measures like **Communication with Doctors**, **Responsiveness**, etc.

3. **Modeling & Insights**:  
   - Lasso, Ridge, and ElasticNet models used to predict Overall Hospital Rating (R² ~ 0.93+).  
   - SHAP analysis reveals the most significant drivers (e.g., **Care Transition**, **Cleanliness**, **Quietness**).

4. **Visualization & Reporting**:  
   - `HCAHPS Patient Survey Analysis.ipynb` presents final results with Plotly and Matplotlib figures.  
   - Exported HTML versions (with and without code) to ensure Plotly graphs display correctly.

---

<a id="key-features"></a>
## 4. Key Features

- **Comprehensive Trends (2014–2023)**:  
  Yearly national averages, measure-level trends, and boxplot distributions.

- **Pandemic Impact Analysis**:  
  Comparison of pre- and post-COVID performance, highlighting a 2–3% score decline in 2021–2022.

- **Driver Identification**:  
  Advanced regression (Lasso, ElasticNet) & SHAP to pinpoint top factors influencing Overall Hospital Rating.

- **State Comparisons**:  
  Detailed breakdown of which states improved or declined, including interactive charts.

---

<a id="technologies"></a>
## 5. Technologies

- **Python**: Pandas, NumPy, Scikit-learn for data processing & modeling  
- **Matplotlib, Seaborn, Plotly**: Visualizing trends and interactive dashboards  
- **SHAP**: Interpreting feature importance in gradient boosting and linear models  
- **Jupyter Notebooks**: Analysis, EDA, and reporting environment  

---

<a id="use-cases"></a>
## 6. Use Cases

- **Hospital Leadership**: Target specific measures (e.g., care coordination, communication about medications) to boost patient satisfaction.  
- **Healthcare Researchers**: Study performance trends over time for evidence-based improvements.  
- **Policy Makers**: Identify and address regional disparities to guide funding and policies.

---