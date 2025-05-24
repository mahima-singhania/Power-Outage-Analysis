# US Electric Grid Power Outage Analysis ⚡

## 📌 Overview
This project analyzes patterns and trends in **power outages** across the **United States** to:
- Understand **outage trends** and regional patterns.
- Assess their **impact on communities**.
- Identify **potential vulnerabilities** in the power grid.

## 🛠 Tool Stack  
🔹 **Power BI** | **MS Excel**  
  
## 🧹Data Processing Steps
### Filtering and Cleaning
- Standardized **restoration dates** (assuming unspecified times = midnight).
- Set **unknown customer numbers** as Zero.
- Set **unknown power loss demand (MW)** to Zero.
- Converted **N/A values in demand loss** to zero.
- Assumed **PG&E answers in affected customers** as unknown.
- Standardized date and time formats*.
- Computed **years since the outage start**.
- **Redefined NERC regions** for simpler analysis:
  - **ERCOT, FRCC, FRCC, MAAC, , MRO, NPCC, PR, RFC, SERC, SPP, TRE, WECC, Multiple**.
- **Categorized event types** into **seven key groups**:
  - **Weather, Natural Disaster, Vandalism, System Operations, Fuel Supply Deficiency, Cyber Attack, Electrical Equipments and Other Causes**.

### 🔍Power Query Transformations
- Unified structure across **Excel sheets** for consolidation.
- Removed **blank rows**.
- Used **Trim function** for text standardization.
- **Split & merged columns** for consistency.
- Modified **incorrect restoration dates** (adjusted values).
- **Renamed column headers** for clarity.
- Inserted **new columns** for calculations.
- Added **calculated fields** to enhance insights.

### 🔵Developed Key Dax Measures 
Created DAX for dynamic calculated such as Total outage, % change in outage, average customers affected, average duration and calculated column for grouped years

### 📊 Visualization 
- **Line Chart Chart:** Shows total cases over time, average customers affected and average hours .
- **Bar Chart:** Displays % of events, events by region etc,.
- **Matrix:** NERC region analysis 
- **Slicers:** Allow filtering by region, date.

## 🔍Findings ⚠️
- **Power outages have increased significantly since 2010**, highlighting growing grid vulnerabilities.
- **Weather-related outages remain the leading cause**, reinforcing the need for better grid resilience.
- **Certain regions experience prolonged outages** due to aging infrastructure and weak restoration processes.
- **Vandalism incidents have surged by 400%**, with a notable rise in the **WECC region**.
- **Power loss and affected customer counts vary widely across states**, indicating uneven outage impacts.

