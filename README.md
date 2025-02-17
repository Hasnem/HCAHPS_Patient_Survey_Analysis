# HCAHPS Patient Satisfaction Analysis (2014–2023)

This repository analyzes **HCAHPS (Hospital Consumer Assessment of Healthcare Providers and Systems)** patient satisfaction data across U.S. hospitals from **2014 to 2023**, identifying trends, key drivers, and the impact of COVID-19 on hospital ratings.

---

## 📌 Table of Contents  
1. [Overview](#overview)  
2. [Data Sources](#data-sources)  
3. [Project Workflow](#project-workflow)  
4. [Key Insights](#key-insights)  
5. [Technologies & Methods](#technologies-methods)  
6. [Use Cases](#use-cases)  

---

<a id="overview"></a>
## 1. Overview  

This analysis explores **HCAHPS patient satisfaction trends** from **2014 to 2023**, focusing on **hospital performance, key drivers of patient experience, and the impact of COVID-19**.

### 🔹 Project Goals  
✔️ Identify **long-term trends** in patient satisfaction scores.  
✔️ Assess **COVID-19's impact** on key measures.  
✔️ Determine **the strongest predictors** of hospital ratings.  

### 🔹 Key Findings  
- **Top Drivers of Patient Satisfaction**:  
  - 📈 **Care Transition**, **Quietness**, and **Cleanliness** have the **strongest influence** on Overall Hospital Rating.  
  - ⚠️ **Communication About Medicines** remains the **weakest-performing measure**, particularly during COVID-19.  

- **Pandemic Impact (2021–2022):**  
  - 📉 **Average hospital ratings declined by ~2–3%** but showed signs of recovery in 2023.  
  - 📊 **Certain states improved** despite nationwide declines, highlighting regional differences in hospital response.

### 🔹 Interactive Dashboard & Code  
Explore **real-time visualizations** in our **interactive dashboard** and **Jupyter Notebook analysis**.

---

<a id="data-sources"></a>
## 2. Data Sources  

1️⃣ **2014–2022 Data**: [Maven Analytics Data Playground](https://mavenanalytics.io/data-playground)  
2️⃣ **2023 Data**: [CMS HCAHPS (Hospital Compare) Archives](https://data.cms.gov/provider-data/archived-data/hospitals)  

### 🔹 Data Processing  
- All datasets were merged, cleaned, and processed using **`data_processor.ipynb`**.  
- The final dataset was used in the **analysis notebook (`HCAHPS Patient Survey Analysis.ipynb`)**.  

---

<a id="project-workflow"></a>
## 3. Project Workflow  

📌 **Step 1: Data Merging & Cleaning**  
- Combined multiple datasets to ensure **consistency** across years.  

📌 **Step 2: Exploratory Data Analysis (EDA)**  
- **Boxplots** and **trend analysis** for Bottom-box, Middle-box, and Top-box responses.  
- **COVID-19 impact analysis** on patient experience scores.  

📌 **Step 3: Statistical & Predictive Modeling**  
- **Hypothesis Testing (T-tests)** confirmed that COVID-19 caused a **statistically significant** drop in scores.  
- **Variance Inflation Factor (VIF) Analysis** ensured no severe multicollinearity in predictors.  
- **Regression Models (Lasso, Ridge, ElasticNet)** predicted Overall Hospital Ratings with **R² > 0.93**.  
- **SHAP Analysis** explained model-driven insights.  

📌 **Step 4: Visualization & Reporting**  
- **Matplotlib, Seaborn, and Plotly** for trend visualizations.  
- Exported **interactive reports** to HTML for better accessibility.  

---

<a id="key-insights"></a>
## 4. Key Insights  

🔹 **Overall Hospital Rating Trends (2014–2023)**  
- **Stable at ~70–72%** pre-pandemic.  
- **Declined by ~2–3% in 2021–2022** due to COVID-19 disruptions.  
- **Partial recovery in 2023** as hospitals adapted to post-pandemic conditions.  

🔹 **State-Level Performance Variations**  
- **Delaware & Hawaii** saw the **steepest declines** (>3%).  
- **North Dakota & Montana** improved despite the pandemic.  
- **State-level policies & healthcare response influenced trends.**  

🔹 **Most Influential Features in Predicting Hospital Ratings**  
| Feature | Impact |
|---------|--------|
| ✅ Care Transition | **Strongest positive driver** |
| ✅ Quietness | **Highly significant** |
| ✅ Cleanliness | **High importance** |
| ❌ Communication About Medicines | **Weakest performer** |
| ❗ Responsiveness of Hospital Staff | **Moderate impact, needs improvement** |

🔹 **COVID-19 Impact on Key Measures**  
| Measure | Avg. Change (Post-COVID) |
|---------|---------------------------|
| 📉 Communication with Nurses | **-2.5%** |
| 📉 Responsiveness of Staff | **-3.1%** |
| 📉 Communication About Medicines | **-3.8%** (largest drop) |
| ✅ Quietness of Environment | **Minimal impact** |

---

<a id="technologies-methods"></a>
## 5. Technologies & Methods  

### 📊 Data Processing & EDA  
- **Pandas, NumPy** – Data cleaning, transformations, and statistical analysis.  
- **Matplotlib, Seaborn, Plotly** – Boxplots, trend visualizations, and interactive charts.  

### 📈 Statistical & Predictive Modeling  
- **Hypothesis Testing** – T-tests for pre/post COVID-19 analysis.  
- **Variance Inflation Factor (VIF) Analysis** – Ensured no severe multicollinearity.  
- **Regression Models (Lasso, Ridge, ElasticNet)** – Predictive modeling (R² > 0.93).  
- **SHAP Analysis** – Explainable AI for feature importance ranking.  

### 📊 Visualization & Reporting  
- **Jupyter Notebooks** – Data exploration and final analysis.  
- **Interactive Dashboards** – Real-time insights via Plotly.  

---

<a id="use-cases"></a>
## 6. Use Cases  

📌 **For Hospital Leadership**  
- Identify **specific measures** (e.g., Care Transition, Cleanliness) to **improve patient satisfaction scores**.  
- Benchmark against **state/national averages** to track progress.  

📌 **For Healthcare Researchers**  
- Study **long-term performance trends** and investigate the effects of policy changes.  
- Use SHAP analysis to **understand how different factors impact patient experience**.  

📌 **For Policy Makers**  
- Identify **regional disparities** in healthcare quality.  
- Allocate **funding & resources** to the areas most in need.  

---

## 🚀 Next Steps  
✔️ Expand the dataset with **hospital-specific trends** (rather than just state/national data).  
✔️ Develop **an interactive dashboard** for real-time insights.  
✔️ Integrate **additional healthcare metrics** (e.g., staffing levels, COVID-19 case data) for deeper analysis.  

---

## 📌 Final Thoughts  
This project provides a **data-driven foundation** for improving patient satisfaction and hospital performance.  
🔹 **By leveraging statistical modeling and visualization**, we can **identify actionable strategies** to enhance healthcare quality.  

🚀 **Check out the notebook & dashboard to explore more insights!**
