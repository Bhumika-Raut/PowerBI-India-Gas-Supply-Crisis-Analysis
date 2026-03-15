# 🇮🇳 India Gas Supply Crisis Analysis (2019–2026)
### Microsoft Power BI Dashboard Project

<img src="images/India Energy Overview.png" width="600" height="420">
<img src="images/LNG Import Dependency.png" width="600" height="420">
<img src="images/Impact on India.png" width="600" height="420">


---

## 📌 Project Overview

This project is an **interactive Power BI dashboard** analyzing India's natural gas supply situation from **2019 to 2026**.

The dashboard focuses on the **2026 LNG supply crisis** caused by global geopolitical conflicts that disrupted international gas supply routes.

The dashboard helps visualize:

- LNG import dependency
- Gas price fluctuations
- State-wise demand and supply risk
- Sector-level gas consumption
- India's energy vulnerability during a global crisis

---

## 🚨 Problem Statement

India heavily depends on **Liquefied Natural Gas (LNG) imports** from countries such as:

- Qatar  
- USA  
- Australia  
- Russia  
- UAE  
- Nigeria  
- Oman  

In **2026**, geopolitical tensions disrupted global LNG supply routes which caused:

- 📈 **Gas prices to increase sharply**
- 📉 **LNG imports to decline**
- ⚡ **Power and fertilizer sectors to face shortages**
- 🗺️ **Multiple Indian states to experience supply risk**

This dashboard analyzes and visualizes the **impact of this crisis on India’s energy system**.

---

# 📊 Dashboard Pages

## Page 1 — India Energy Overview

A national-level summary of India's gas situation.

**Visuals Included**

- KPI Cards  
  - Total LNG Imports  
  - Average Gas Price  
  - Domestic Production  
  - Crisis Status  

- Line Chart  
  **Gas Price Trend (2019–2026)**

- Area Chart  
  **LNG Imports Over Time**

- Bar Chart  
  **Gas Demand vs Domestic Production**

- Slicers  
  - Year  
  - Import Country

---

## Page 2 — LNG Import Dependency

This page analyzes **which countries India depends on for LNG supply**.

**Visuals Included**

- 🌍 World Map  
  LNG supplier countries

- 📊 Bar Chart  
  LNG Imports by Country

- 🍩 Donut Chart  
  Import share by country

- 📋 Table  
  Top supplier countries and disruption level

- Slicer  
  Year

---

## Page 3 — Impact on India

Shows **how the gas crisis affects Indian states and economic sectors**.

**Visuals Included**

- 🗺️ India Map  
  State-wise gas demand

- 📊 Column Chart  
  Gas consumption by sector  
  (Power, Fertilizer, Industry, Transport, City Gas)

- 📈 Line Chart  
  Demand vs Domestic Production

- 🎯 Gauge  
  Supply Gap (BCM)

- Slicers  
  - Year  
  - State  
  - Sector

---

---

# 📂 Datasets

### Dataset 1 — LNG Imports

Columns:

- Year (2019–2026)
- Import Country
- LNG Imports (Million MT)
- Gas Price (USD/MMBtu)
- Supply Disruption Level
- Crisis Status

**Rows:** 343

---

### Dataset 2 — Gas Consumption in India

Columns:

- Year
- State
- Sector
- Gas Demand (BCM)
- Domestic Production (BCM)
- Storage Level %
- Supply Risk Level

**Rows:** 2050

---

# 🛠️ Technologies Used

- **Microsoft Power BI Desktop** — Dashboard creation
- **Power Query** — Data cleaning
- **DAX** — Calculations and measures
- **CSV Files** — Data source

---

# 🧮 DAX Measures
Total LNG Imports =
SUM(LNG_Imports_India_2019_2026[LNG_Imports_Million_MT])

Avg Gas Price =
AVERAGE(LNG_Imports_India_2019_2026[Gas_Price_USD_per_MMBtu])

Is Crisis Year =
IF(MAX(LNG_Imports_India_2019_2026[Year]) = 2026, "CRISIS", "Normal")

Total Gas Demand =
SUM(India_Gas_Consumption_2019_2026[Gas_Demand_BCM])

Total Domestic Production =
SUM(India_Gas_Consumption_2019_2026[Domestic_Production_BCM])

Supply Gap BCM = [Total Gas Demand] - [Total Domestic Production]


---

# 🚀 How to Use

1️⃣ Download the repository.

2️⃣ Open the project in **Microsoft Power BI Desktop**.

3️⃣ Open the file:


4️⃣ Explore the dashboard using slicers.

---

## ⚠️ Important Navigation Tip

When opening the dashboard **in edit mode**, navigation buttons work differently.

👉 You must press:

**CTRL + Click**

to move between pages.

---

# 📈 Key Insights

- 🔴 **2026 Crisis Impact:** Gas prices increased more than 2× compared to 2025  
- 📉 **Import Drop:** Gulf LNG supply dropped significantly  
- 🇺🇸 **USA Imports Increased:** Alternative supply source  
- ⚡ **Most Affected Sectors:** Power and Fertilizer  
- 🗺️ **High Risk States:** Delhi, Punjab, Uttar Pradesh  
- 📊 **Supply Gap:** Domestic production covered less than 30% of demand

---

# 🎓 Project Context

Developed as part of the **Microsoft Elevate AICTE Internship Program (2026)**.

Domain: **Energy Analytics**  
Tool: **Microsoft Power BI Desktop**

---

# 👩‍💻 Author

**Bhumika Raut**

---

Built with ❤️ using Microsoft Power BI
