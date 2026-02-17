# GDP-Per-Capita-Countries


## Project Overview
This project leverages Python to conduct a comprehensive analysis of global financial trends, focusing specifically on GDP per capita as a key indicator of economic performance. By examining data from over 200 countries, the project explores how wealth is distributed globally, identifies patterns across regions, and investigates the relationships between different economic metrics and country characteristics. 


##  Table of GDP-Per-Capita-Countries 
<img width="536" height="227" alt="GDP PER CAPITA TABLE" src="https://github.com/user-attachments/assets/bc8bfef6-b68f-42e6-b348-cca52839352e" />

##  Correlation of GDP-Per-Capita-Countries <img width="621" height="268" alt="GDP CORRELATION" src="https://github.com/user-attachments/assets/45a92c46-0fc0-4f7c-9971-6699163bc799" />

##  Frequency of IMF Estimate
<img width="298" height="251" alt="image" src="https://github.com/user-attachments/assets/cd1d85c7-42c2-4cc9-a6d1-74a8093dd013" />

[Data Source](https://github.com/ezemeju-lgtm/GDP-Per-Capita-Countries/blob/main/GDP%20(nominal)%20per%20Capita.csv)

View code on google collab [here](https://colab.research.google.com/drive/12MYEzihkdNYdxIEWaRag-ISjjLFGk_qm?authuser=0#scrollTo=x1rHlxMrVp4E)
# 🌍 Global GDP Per Capita Analysis

## 📋 Project Purpose
This project focuses on the **analysis of global GDP per capita** using a comprehensive dataset compiled from three major international sources: the **International Monetary Fund (IMF)** , the **World Bank**, and the **United Nations (UN)** . The goal is to **clean, explore, and compare** these estimates to understand global wealth distribution, identify economic patterns, and derive insights into the **economic performance of countries and regions** across the world.

---

## 📦 The Dataset
- **Source:** Compiled dataset combining estimates from IMF, World Bank, and UN
- **Content:** GDP per capita figures for **223 countries and territories**
- **Timeframe:** Estimates range from **2007 to 2023**, with most recent data around **2021–2023**
- **Structure:** One row per country/territory with multiple estimate columns

### Key Columns:
| Column | Description |
|--------|-------------|
| `Country/Territory` | Name of the country or territory |
| `UN_Region` | Regional classification (e.g., Europe, Asia, Americas, Africa, Oceania) |
| `IMF_Estimate` | GDP per capita estimate from the IMF |
| `IMF_Year` | Year of the IMF estimate |
| `WorldBank_Estimate` | GDP per capita estimate from the World Bank |
| `WorldBank_Year` | Year of the World Bank estimate |
| `UN_Estimate` | GDP per capita estimate from the United Nations |
| `UN_Year` | Year of the UN estimate |

---

## 🧹 Data Cleaning & Wrangling Process
Before meaningful analysis could begin, the raw dataset required significant preparation. This involved:

### 1. Handling Missing Values
- Many territories have **zero values** or missing estimates from certain sources.
- Small territories and dependencies (e.g., Bermuda, Cayman Islands, Faroe Islands) often only have data from one source.
- Some countries have **inconsistent year coverage** across sources.

**Approach:**
- Identify gaps and decide whether to exclude, estimate, or flag missing data.
- Consider using the most reliable available source for each country.

### 2. Standardising Years
- Estimates come from **different years** (2007–2023).
- Direct comparisons require either:
  - Using the **most recent available data** for each country, or
  - Focusing on a **specific year** where coverage is strong (e.g., 2021).

### 3. Addressing Data Quality Issues
- Some estimates appear **inconsistent** across sources (e.g., Venezuela: World Bank 2014 estimate of $15,976 vs. UN 2021 estimate of $3,965).
- A few countries have **zero values** that may indicate missing data rather than true zero GDP.
- Small discrepancies between sources are expected, but large differences need investigation.

### 4. Creating Derived Metrics
- **Primary estimate** – Choose the most reliable or recent source for analysis.
- **Source comparison** – Calculate differences between IMF, World Bank, and UN estimates.
- **Regional groupings** – Aggregate data by `UN_Region` for regional analysis.
- **Wealth categories** – Create bands (e.g., low income, middle income, high income) for segmentation.

---

## 🔍 Key Questions the Analysis Seeks to Answer

### For Economists & Policy Researchers:
- Which countries have the **highest and lowest** GDP per capita?
- How does **wealth distribution vary across regions** (Europe vs. Africa vs. Asia)?
- Are there **significant discrepancies** between IMF, World Bank, and UN estimates?
- Which countries show the most **volatility or inconsistency** in reported figures?

### For Regional Analysis:
- Which regions are the **wealthiest** on average?
- What is the **spread of wealth** within each region (inequality)?
- Are there **geographic patterns** to economic performance?

### For Data Quality Assessment:
- How **reliable** are the different sources for different countries?
- Which countries have the **most complete data coverage**?
- Are there notable **outliers or data anomalies** that require explanation?

---

## 📊 Expected Outputs & Insights
The final deliverables will include:

- **Clean, structured dataset** ready for further analysis or visualisation
- **Summary statistics** including:
  - Top 10 richest countries (by GDP per capita)
  - Bottom 10 poorest countries
  - Regional averages and medians
  - Global distribution of wealth
- **Visualisations** showing:
  - Bar charts of top countries by GDP per capita
  - Regional comparisons (average GDP per capita by continent)
  - Distribution plots showing global inequality
  - Source comparison charts highlighting discrepancies between IMF, World Bank, and UN
  - World map with colour-coded GDP per capita bands
- **Written summary report** highlighting:
  - Key findings and patterns
  - Notable outliers and anomalies
  - Data quality observations
  - Limitations and caveats

---

## 🌍 Who Will Benefit?

| Stakeholder | How They Benefit |
|-------------|------------------|
| **Economists & Researchers** | Access to cleaned, comparable GDP data for analysis |
| **Policy Makers** | Understanding of global wealth distribution and regional disparities |
| **Students & Educators** | Teaching resource for economics and data analysis |
| **Journalists & Media** | Data for stories on global inequality and economic development |
| **International Organisations** | Insights for aid allocation and development planning |
| **General Public** | Accessible overview of global economic landscape |

---

## ⚠️ Limitations & Caveats
- **Different years** – Estimates come from different years, so direct comparisons are imperfect.
- **Small territories** – Many small islands and dependencies have limited or no data.
- **Source discrepancies** – Significant differences between sources for some countries highlight data reliability challenges.
- **Nominal vs. PPP** – This is **nominal** GDP per capita, not adjusted for purchasing power parity (PPP).
- **Currency** – All figures are in **current USD** (not inflation-adjusted), so comparisons across years should be cautious.

---

## 📁 Repository Structure
