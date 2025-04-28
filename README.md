# Urban Mobility Insights with Python (NYC Taxi Trips)
Data can optimize taxi routes and reduce congestion in bustling citie. In this project I analyzed NYC taxi data to identify optimal zones for efficient operations.

Link to the main file for analysis : https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

**Here’s what the code does:**  
1️⃣ **Data Loading & Preprocessing**  
- Efficiently loads Parquet trip data and CSV zone data with **error handling** for robustness.  
- Merges pickup/dropoff zones, calculates trip durations/speeds, and filters outliers (e.g., unrealistic speeds).  

2️⃣ **Demand & Congestion Analysis**  
- Identifies high-demand zones by trip volume, passenger count, and distance.  
- Quantifies congestion impact using surcharge data and average speeds.  

3️⃣ **Route Optimization**  
- Combines demand and congestion metrics into a weighted **optimization score**.  
- Ranks top zones using a normalized scoring system to balance efficiency and profitability.  

4️⃣ **Visualization**  
- Uses `seaborn` and `matplotlib` to create an insightful scatter plot, highlighting the trade-off between demand and congestion.  

**Tech Stack & Best Practices:**  
- **PyArrow** for fast Parquet file handling.  
- **Pandas** for seamless data merging/aggregation.  
- **Defensive Programming** with try/except blocks and data validation.  
- **Modular Design** for reusability (functions for ETL, analysis, and visualization).  
