🇮🇳 India Gas Supply Crisis Analysis (2019–2026)
A Microsoft Power BI Dashboard Project


📌 Project Overview
This project is an interactive Power BI dashboard that analyzes India's natural gas supply crisis from 2019 to 2026. The dashboard focuses on the impact of the 2026 global LNG supply disruption caused by geopolitical conflicts affecting key gas export routes — and how it impacted India's energy security, import dependency, state-wise demand, and sector-level consumption.

🚨 Problem Statement
India's growing energy demand heavily relies on Liquefied Natural Gas (LNG) imports from countries like Qatar, USA, Australia, Russia, UAE, Nigeria, and Oman. In 2026, a major geopolitical crisis disrupted global LNG supply routes, causing:

📈 Gas prices to spike dramatically
📉 LNG import volumes to drop sharply
⚡ Power, fertilizer, and industrial sectors to face severe shortages
🗺️ Multiple Indian states to reach critical supply risk levels

This dashboard visualizes these trends and helps analysts understand India's energy vulnerability.

📊 Dashboard Pages
Page 1 — India Energy Overview

National-level summary of India's gas situation (2019–2026)

VisualDescription4 KPI CardsTotal LNG Imports, Avg Gas Price, Domestic Production, Crisis StatusLine ChartGas Price Trend — showing 2026 spikeArea ChartLNG Imports Over Time — showing 2026 dropBar ChartGas Demand vs Domestic Production comparisonSlicersYear, Import Country

Page 2 — LNG Import Dependency

Analysis of which countries India depends on for LNG

VisualDescriptionWorld MapLNG supplier countries with bubble sizes by import volumeBar ChartLNG Imports by Country with disruption level colorsDonut ChartImport share percentage by countryTableTop 3 countries — Import volume, Gas price, Disruption levelSlicerYear

Page 3 — Impact on India

How the crisis affects Indian states and economic sectors

VisualDescriptionIndia MapGas demand highlighted by stateColumn ChartGas consumption by sector (Power, Fertilizer, Industry, Transport, City Gas)Line ChartDemand vs Domestic Production — widening gap in 2026GaugeSupply Gap BCM — risk indicatorSlicersYear, State, Sector

📁 Repository Structure
India-Gas-Supply-Crisis-Analysis-PowerBI/
│
├── 📊 India_Gas_Supply.pbix              # Main Power BI Dashboard File
│
├── 📄 Data/
│   ├── LNG_Imports_India_2019_2026.csv   # Dataset 1 — LNG Import data (343 rows)
│   └── India_Gas_Consumption_2019_2026.csv # Dataset 2 — Gas Consumption data (2050 rows)
│
├── 🖼️ Screenshots/
│   ├── Page1_India_Energy_Overview.png
│   ├── Page2_LNG_Import_Dependency.png
│   └── Page3_Impact_on_India.png
│
└── 📖 README.md

📂 Datasets
Dataset 1 — LNG Imports Affecting India
ColumnDescriptionYear2019–2026Import_CountryQatar, USA, Australia, Russia, UAE, Nigeria, OmanLNG_Imports_Million_MTImport volume in Million Metric TonnesGas_Price_USD_per_MMBtuGas price in USD per MMBtuSupply_Disruption_LevelLow / Medium / HighCrisis_StatusNormal / Watch / Elevated / CRISIS
Rows: 343 | Period: 2019–2026

Dataset 2 — India Gas Consumption Impact
ColumnDescriptionYear2019–2026State10 Indian states including Gujarat, Maharashtra, Delhi, etc.SectorPower, Fertilizer, Industry, Transport, City GasGas_Demand_BCMGas demand in Billion Cubic MetresDomestic_Production_BCMDomestic production in BCMStorage_Level_PercentageStorage level %Supply_Risk_LevelLow / Medium / High / Critical
Rows: 2,050 | Period: 2019–2026

🛠️ Technology Used
TechnologyPurposeMicrosoft Power BI DesktopDashboard creation and visualizationDAX (Data Analysis Expressions)Custom measures and calculationsPower QueryData transformation and cleaningCSV FilesData source

🧮 DAX Measures Created
daxTotal LNG Imports = SUM(LNG_Imports_India_2019_2026[LNG_Imports_Million_MT])

Avg Gas Price = AVERAGE(LNG_Imports_India_2019_2026[Gas_Price_USD_per_MMBtu])

Is Crisis Year = IF(MAX(LNG_Imports_India_2019_2026[Year]) = 2026, "CRISIS", "Normal")

Total Gas Demand = SUM(India_Gas_Consumption_2019_2026[Gas_Demand_BCM])

Total Domestic Production = SUM(India_Gas_Consumption_2019_2026[Domestic_Production_BCM])

Supply Gap BCM = [Total Gas Demand] - [Total Domestic Production]

🎨 Dashboard Theme
ElementColor CodePage Background#0D1B2A (Deep Navy)Card Background#0D1B2ABorders & Accents#00C8FF (Cyan Glow)Title Banner#1B3A6B (Dark Blue)Crisis Alert#FF0000 (Red)Chart Lines#00C8FF (Cyan)

🚀 How to Use

Clone the repository:

bashgit clone https://github.com/YOUR_USERNAME/India-Gas-Supply-Crisis-Analysis-PowerBI.git

Open Power BI Desktop

Download free from: https://powerbi.microsoft.com/desktop


Open the dashboard file:

Open India_Gas_Supply.pbix in Power BI Desktop


Explore the dashboard:

Use the Year slicer to filter by specific year
Select 2026 to see full crisis impact
Use **Ctrl + Click** on navigation buttons to switch pages (in edit mode)
In reading/presentation mode, click normally to navigate




📈 Key Insights

🔴 2026 Crisis Impact: Gas prices spiked over 2x compared to 2025 levels
📉 Gulf Route Disruption: Qatar, UAE, and Oman imports dropped by ~55% in 2026
🇺🇸 USA Gains Share: US LNG exports to India increased as alternative supply
⚡ Power & Fertilizer sectors most affected by supply shortage
🗺️ Delhi, Punjab, UP reached Critical supply risk levels in 2026
📊 Supply Gap: Domestic production covered less than 30% of demand in 2026


🎓 Project Context
This project was developed as part of the Microsoft Elevate AICTE Internship Program (Feb 2026).

Tool: Microsoft Power BI Desktop
Domain: Energy Analytics
Type: Capstone Project


👩‍💻 Author
Bhumika Raut

📄 License
This project is for educational purposes as part of the Microsoft Elevate AICTE Internship Program.

Built with ❤️ using Microsoft Power BI
