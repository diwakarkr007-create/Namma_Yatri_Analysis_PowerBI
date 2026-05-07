# Namma_Yatri_Analysis_PowerBI
End-to-end Power BI dashboard analyzing ride-hailing metrics, conversion funnels, and driver earnings for Namma Yatri.
https://app.powerbi.com/groups/me/reports/ebcff413-5a13-4ac0-8deb-c7e1e4d75148/e6e8b5b3b70a309731e3?experience=power-bi
# Namma Yatri Ride-Hailing Analysis 🚖

## 📊 Live Project Link
🚀 **[Click here to view the Interactive Dashboard](<iframe title="DV_Namma_Yatri_Cab_Diwakar_Kumar" width="1024" height="804" src="https://app.powerbi.com/view?r=eyJrIjoiZTI5MWI2ZGYtOTkwZi00MTk2LWJhMGUtYTBjMWYzZDZmZWNmIiwidCI6ImYxODZiYjUxLWMyNDMtNDA0OC1iNDA4LTliMjhhNmU1MjVlZiJ9" frameborder="0" allowFullScreen="true"></iframe>)**

---
# 🚖 Namma Yatri Operational Analytics & Business Intelligence

## 📌 Project Overview
This project is an advanced Data Analytics and Business Intelligence dashboard built using Power BI. It analyzes the "Search-to-Success" journey of a ride on the Namma Yatri open mobility platform, identifying critical revenue leakages, operational bottlenecks, and opportunities for supply-side optimization.

## 🏗️ Data Architecture & ETL (The "Merged Table" Approach)
To establish a highly performant **Star Schema** and a "Single Source of Truth", the data model was heavily optimized:
* **Consolidated Fact Table:** Merged the raw `Trip Details` (Intent layer) and `Trips` (Execution layer) tables using a Left Outer Join on `tripid`.
* **Optimization:** Deleted the original fragmented tables post-merge to reduce redundancy, isolate data, and enhance DAX calculation speeds.
* **Type Casting:** Standardized `tripid` to Text/String to prevent auto-aggregation, and cast financial metrics (fare, distance) to Floats/Decimals.
* **Dynamic DAX:** Engineered complex DAX measures leveraging `SWITCH` logic and 'What-If' parameters for real-time visual filtering.

## 📊 Key Business Insights & Metrics
* **The Abandonment Crisis:** Identified a severe **40.91% drop-off rate** before booking, translating to an estimated **₹900.39K in Revenue Loss**.
* **Opportunity Gap:** Calculated an Opportunity Gap score of **1.178** (For every completed trip, 1.17 potential rides are lost to supply friction).
* **Conversion Funnel:** Mapped the user journey from 2,161 searches to 983 completed trips, yielding an overall **45.49% Success Rate**.
* **Cancellation Dynamics:** Customer cancellations sit at **7.27%**, while Driver cancellations are at **6.34%**.

## 🗺️ Geospatial & Temporal Hotspots
* **Volume Engine:** **Ramanagaram** records the highest search intent and completed trips, requiring immediate supply density optimization.
* **Premium Revenue Driver:** **Bangalore South** generates the highest EBITDA/fare per trip due to longer average ride distances.
* **Friction Zone:** **Mahadevapura** suffers from the highest cancellation rates, primarily driven by traffic corridors and "dead miles".
* **The Midnight Surge:** Temporal analysis revealed a critical shift-end peak demand at **12 AM - 1 AM (53 trips)**, necessitating targeted late-night driver incentives.

## 💡 Strategic Recommendations
1. **Localized Supply Density:** Deploy targeted driver onboarding in Ramanagaram to capture the 40.91% abandoned intent.
2. **Midnight Surge Pricing:** Implement 12 AM - 1 AM supply bonuses to ensure availability during the daily peak.
3. **Reliability Bonuses:** Address the traffic-heavy Mahadevapura zone with specific fulfillment bonuses to lower the combined 13.6% cancellation risk.

## 🛠️ Technologies Used
* **BI Tool:** Power BI
* **Data Modeling:** Star Schema, ETL (Power Query)
* **Languages:** DAX (Data Analysis Expressions)
* **Advanced Features:** Dynamic Slicers, Parameter Engineering, Conditional RAG Formatting.

---
*Developed as part of an advanced Data Science and Analytics portfolio, focusing on translating raw operational logs into strategic business decisions.*

---
**Author:** Diwakar Kumar  
**Connect with me:** [linkedin.com/in/diwakar-kumar-93531b371]
