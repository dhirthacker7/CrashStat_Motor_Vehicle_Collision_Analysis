# **CrashStat: Motor Vehicle Collision Data Warehouse**

CrashStat analyzes motor vehicle collision data from New York, Chicago, and Austin to identify accident patterns, risk factors, and safety insights. The project implements a complete data warehouse solution with ETL pipelines and interactive dashboards to answer critical questions about traffic safety.

---

## **Objectives**

- Quantify accident volumes across three cities
- Identify top high-risk areas and most fatal locations
- Analyze injury and fatality statistics by city
- Assess pedestrian involvement and safety
- Examine temporal patterns (time of day, day of week, seasonality)
- Identify common contributing factors

---

## **Data Sources**

### **New York City**
- [NYC Open Data](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95)

### **Chicago**
- [City of Chicago Data Portal](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if)

### **Austin**
- [City of Austin Data](https://data.austintexas.gov/Transportation-and-Mobility/Austin-Crash-Report-Data-Crash-Level-Records/y2wy-tgr5)

---

## **Implementation**

![Architecture_Diagram](Architecture_Diagram.png)

### **Phase 1: Data Profiling and Staging**
- Profiled data using Python (ydata-profiling) and Alteryx
- Identified quality issues: missing values, inconsistent formats, duplicates
- Created staging tables with audit columns in SQL Server

### **Phase 2: ETL Pipeline and Integration**
- Built ETL workflows in Talend Studio
- Standardized, cleansed, and transformed data
- Loaded dimensional model with SCD Type 2 implementation
- Validated data integrity with SQL queries

### **Phase 3: Business Intelligence**
- Developed dashboards in Power BI and Tableau
- Created interactive visualizations for all analytical goals
- Implemented drill-down and filtering capabilities

---

## **Dashboard**
[Power BI](https://app.powerbi.com/groups/me/reports/dda3d0e1-ed89-47eb-a83d-4058f6991367/ReportSection?experience=power-bi)
### **1. Overview and Temporal Analysis**
Displays total accident counts by city (3.04M total), severity breakdown (4,964 injuries, 893K total injury count), and time-based analysis showing seasonal trends. The central visualization reveals peak accident periods throughout the year with injury vs. fatal comparisons.
<img width="1200" height="672" alt="image" src="https://github.com/user-attachments/assets/326a72ea-ff81-4713-af36-9cee3a8aed84" />

---

### **2. Geographic and Pedestrian Analysis**
Features an interactive map highlighting collision hotspots across the three cities, motor vehicle deaths and injuries by location, and pedestrian accident trends over time. Shows concentration of accidents in urban centers and tracks pedestrian involvement patterns.
<img width="1403" height="792" alt="image" src="https://github.com/user-attachments/assets/32bee90f-4792-4fdd-92d5-2459d2084aa0" />


---

### **3. Contributing Factors Analysis**
Comprehensive breakdown of the most common contributing factors leading to accidents. Lists top causes including driver inattention, failure to yield, and following too closely. Shows accident counts by data source and identifies the top 5 street names with highest accident frequency (1,695 motor vehicle deaths, 466K person vehicle injuries).
<img width="1197" height="670" alt="image" src="https://github.com/user-attachments/assets/3e49fa74-c8b2-4d8a-ba1c-c236bbe73b1e" />

---

## **Technologies Used**

| Category | Technologies |
|----------|-------------|
| **Data Profiling** | Python (ydata-profiling), Alteryx |
| **ETL** | Talend Studio |
| **Database** | SQL Server, Microsoft Excel |
| **Visualization** | Power BI |
| **Version Control** | Git, GitHub |

---

## *Key Insights*
Through comprehensive analysis of collision data across three major cities, CrashStat has uncovered critical findings:

- **Geographic Hotspots:** Identified top accident-prone areas in New York, Chicago, and Austin, with concentrated clusters in downtown corridors and major intersections
- **Temporal Patterns:** Peak accident periods occur during evening rush hours (5-7 PM) and Friday evenings, with distinct weekday vs. weekend patterns
- **Seasonal Trends:** Higher collision frequency during winter months, with weather conditions significantly impacting accident rates
- **Contributing Factors:** Most common causes include driver inattention/distraction, failure to yield right of way, following too closely, and unsafe speed
- **Pedestrian Safety:** Analyzed pedestrian involvement rates across cities, revealing critical zones requiring enhanced safety measures
- **Severity Analysis:** Examined injury and fatality statistics at both city-specific and aggregate levels, identifying high-risk locations requiring immediate intervention
- **Motorist Impact:** Tracked injury and death rates among motorists, providing insights for targeted safety campaigns

---

## **Author**   
[Dhir Thacker](https://www.linkedin.com/in/dhirthacker7/)
