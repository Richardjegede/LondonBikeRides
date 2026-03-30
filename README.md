**🚲 London Bike Rides Interactive Dashboard with Tableau**

**📌 Problem Statement**
London’s bike-sharing system generates massive amounts of data, yet it is difficult for city planners and transport authorities to identify the specific environmental and temporal factors that drive ridership.
Understanding how weather conditions (temperature, humidity, wind speed) and time-based variables (seasons, holidays, weekends) impact bike usage is critical for optimizing bike distribution and infrastructure maintenance. Without a centralized visual tool, spotting long-term growth trends or sudden shifts in public behavior remains a manual and complex task.

**💡 The Solution**
The London Bike Rides Tableau Dashboard transforms raw Kaggle dataset records into a high-fidelity interactive experience. 
It allows stakeholders to perform deep-dives into ridership patterns across different time scales.
By utilizing Moving Averages and Heatmaps, the dashboard provides a clear view of peak usage periods, enabling data-driven decisions for urban mobility and public transport planning.

**🛠️ Project Workflow (Tableau Development)**

-Data Acquisition: I explored, access and manipulated the data from kaggle using pandas library from python and extracted the (CSV format) with zipfile library in python.
<img width="1366" height="385" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/d21ae933-9215-440b-9dff-1988a378c936" />
**Extracting the file from kaggle**
<img width="1366" height="654" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/641045b3-2e17-4d14-8b69-634eead8aa5d" />

-Data Transformation: Created Calculated Fields to transform numerical weather codes into human-readable categories (e.g., "Clear," "Cloudy," "Rainy").
-Time-Series Analysis: Developed a primary line chart with a User-Defined Parameter for Moving Averages (e.g., 7-day or 30-day) to smooth out daily fluctuations.
-Correlation Mapping: Built a "Weather vs. Usage" matrix to analyze the impact of temperature (T1) and "feels-like" temperature (T2) on total rides.
-Dashboard Architecture: Created 5 visualisations and linked everything together to produce a compelling tableau dashboard and i also Designed a tiled layout focusing on the "F-Pattern" for readability, ensuring the most critical KPIs are in the top-left.

*Total Number of bike rides*
<img width="1353" height="701" alt="Screenshot (77)" src="https://github.com/user-attachments/assets/714b5255-ae22-4d26-ae22-88af5e1aa3a1" />

*Moving Average*
<img width="1353" height="701" alt="Screenshot (78)" src="https://github.com/user-attachments/assets/7d2c8731-2a58-45ef-bd46-dcb275f26368" />

*Temperature vs The wind speed heat map*
<img width="1353" height="701" alt="Screenshot (79)" src="https://github.com/user-attachments/assets/e2812ea9-0783-4bd3-a100-32fd395c7194" />

*The Weather Tool Tip
<img width="1353" height="710" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/ac73c176-7485-4792-8b04-9398608c237c" />

*The Hour Tool Tip*
<img width="1353" height="710" alt="Screenshot (81)" src="https://github.com/user-attachments/assets/e7a37994-7daf-49c0-8140-601cfc13896e" />


-Interactivity: Implemented Dashboard Actions and Dynamic Tooltips so users can hover over specific data points for granular details.
*The Interactive Dashboard*
<img width="1353" height="723" alt="Screenshot (83)" src="https://github.com/user-attachments/assets/db65a7f6-3f24-4915-8b1f-ebb3c6f41ee0" />


**📊 Key Insights**

-Weather Impact: Ridership shows a direct positive correlation with temperature, but a sharp decline once humidity crosses the 70% threshold.
-Peak Periodicity: Significant spikes occur during weekday morning and evening rush hours, while weekend usage is more evenly distributed across the afternoon.
-Seasonal Trends: Summer months account for nearly 45% of total annual rides, highlighting a strong seasonal dependency for casual riders.
-Environmental Resilience: Wind speed has a negligible impact on ridership compared to precipitation levels.

**🛠️ Challenges & Customizations**

-Dynamic Moving Averages: A major customization was creating a parameter that allows the end-user to toggle the "smoothing" of the data. 
This helps distinguish between a one-day spike and a genuine upward trend.
-Weather Icon Integration: Used custom shapes to represent different weather conditions, making the dashboard more intuitive for non-technical users.

**🚀 Future Roadmap**

-Predictive Modeling: Integrating a Tableau Forecast model to predict ridership for the next 6 months.
-Live Data Connection: Transitioning from a static CSV to a live Web Data Connector (WDC) for real-time monitoring.
-Geospatial Expansion: Mapping specific docking station coordinates to identify high-traffic "hotspots.

**🎓 Key Learnings**

-Advanced Tableau Logic: Mastered the use of Level of Detail (LOD) Expressions for complex aggregations.
-UX/UI Design: Learned the importance of whitespace and Data-Ink Ratio to prevent visual clutter in dense datasets.
-Domain Specifics: Gained a deep understanding of urban micro-mobility trends and how environmental data influences public behavior.
-Solo Project Success: Delivered this comprehensive analysis independently, from data cleaning to final presentation. 📈🔥
