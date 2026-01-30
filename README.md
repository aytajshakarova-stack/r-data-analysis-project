# r-data-analysis-project
Academic data analysis project using R and Statistics

# Data Analytics Final Project – Sales Transactions Analysis

##  Project Overview
This project was developed as a **comprehensive data analytics case study** aimed at analyzing large-scale sales transaction data.  
The primary objective is to **understand sales behavior, revenue drivers, data quality issues, and anomalies**, and to demonstrate a **full analytical workflow** from raw data to interpretable insights.

The project reflects **real-world data challenges**, including noisy text fields, missing values, duplicated mappings, and extreme outliers, and shows how these issues can be handled analytically rather than simply removed.

---

## Purpose of the Analysis
The analysis was designed to answer the following analytical and business-oriented questions:

- How is overall sales performance distributed across time, products, and POS locations?
- Which products generate the highest number of transactions versus the highest revenue?
- Are there unusual transaction patterns or extreme values that indicate anomalies?
- What factors most strongly influence revenue and profit?
- Can revenue be reasonably explained using interpretable predictive models?

These questions are typical for **retail analytics, business intelligence, and academic data analysis**, making the project suitable for both university evaluation and professional portfolios.

---

##  Data Description
The analysis is based on **transaction-level retail data**, where:

- Each row represents **one transaction (receipt-level granularity)**  
- Quantitative variables include:
  - Quantity sold
  - Unit price
  - Revenue
  - Profit
  - Profit margin
- Categorical variables include:
  - Product name
  - Product type (FOOD / NON-FOOD)
  - POS location
  - Time period

An additional mapping dataset is used to enrich transaction data with revenue and profit-related attributes, requiring careful preprocessing and controlled joining.

---

##  Data Preparation & Cleaning
A major focus of the project is **data preparation**, reflecting real-world analytical practice.

Key steps include:

- Verification of data structure and variable types  
- Detection and inspection of missing values  
- Cleaning and normalization of text-based fields (product names, POS identifiers)  
- Creation of derived variables:
  - `period` (year–month format)
  - `revenue`
  - `profit`
  - `profit_margin`
- Aggregation of duplicated records in mapping data  
- Controlled joining of transactional and mapping datasets  

These steps ensure analytical accuracy, reproducibility, and reliable interpretation.

---

##  Descriptive & Exploratory Analysis
The exploratory analysis focuses on understanding overall data behavior and structure:

- Summary statistics and distribution analysis  
- Total number of transactions, total quantity sold, and total revenue  
- Product type comparison (FOOD vs NON-FOOD):
  - Transaction frequency
  - Revenue distribution  
- Identification of top-performing products:
  - Top products by transaction count
  - Top products by total revenue  
- POS-level revenue concentration analysis  

Visualizations such as **bar charts, boxplots, and histograms** are used extensively to support insights.

---

##  Anomaly & Outlier Analysis
Instead of automatically removing extreme values, this project explicitly **investigates anomalies**:

- Abnormally high daily transaction volumes  
- Extreme revenue values across time  
- Product-type-specific revenue outliers  
- Negative and extremely high profit margin values  

These observations are interpreted as **potential business events, operational irregularities, or exceptional transactions**, and are preserved to maintain analytical transparency.

---

##  Correlation & Predictive Modeling
To identify revenue drivers, the project includes:

- Correlation analysis between:
  - Revenue
  - Quantity
  - Unit price
  - Profit
  - Time period  
- Interpretation of strong and weak relationships  
- Construction of an interpretable linear regression model:

---

##  Key Insights
- Revenue is strongly driven by quantity sold and moderately influenced by unit price  
- A small number of products and POS locations generate a disproportionate share of total revenue  
- Revenue distributions are right-skewed, indicating the presence of high-value transactions  
- Extreme profit margin values may indicate non-standard or risky transactions worthy of further investigation  

---

## Tools & Libraries
- **R**
- `tidyverse`
- `dplyr`
- `ggplot2`
- `stringr`
- `lubridate`
- `R Markdown`

---

##  How to Reproduce the Analysis
1. Clone or download this repository  
2. Open the `.Rmd` file in RStudio  
3. Install the required libraries  
4. Knit the file to generate the HTML report  

---

##  Repository Contents
- `DA Yekun Layihə AytajSh 20260109.Rmd` – Main analysis code and documentation  
- `DA Yekun Layihə AytajSh 20260109.html` – Rendered analytical report  

 **Note:**  
Due to data confidentiality and size limitations, the raw datasets are not publicly shared.

---

##  Author
**Aytaj Shakarova**  
Data Analytics | Applied Data Analysis  
Project prepared for academic evaluation and portfolio use


