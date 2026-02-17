# 🌦️ Power BI Weather Dashboard (Weather API Integration)

##  Project Overview

This project demonstrates how to connect **Power BI** with a Weather API, transform the data, model multiple related tables, and build an interactive weather dashboard.

The objective of this project was to practice:

- API data extraction
- Data transformation using Power Query
- Data modeling and relationships
- Dashboard design and visualization in Power BI

---

##  Data Source

Weather data was fetched using a public Weather API and connected directly to Power BI.

🎥 Tutorial Reference:  
https://youtu.be/P8HB8dMfKNc?si=4CZlzm46Bs7sdBKV

---

##  Data Transformation Process

After connecting to the API, a **Master Table** was created containing the raw weather dataset.

From the master dataset, separate tables were created for better structure and modeling:

- **Current**
- **Forecast_Day**
- **Forecast_Hour**
- **Location**

Only relevant and allocated columns were kept in each table to normalize the structure and improve performance.

---

##  Data Modeling

The data model was built by creating relationships using:

**Location Name**

The following tables were connected using Location Name:

- Current
- Forecast_Day
- Forecast_Hour
- Location

This ensured:

- Consistent filtering
- Proper slicer behavior
- Accurate cross-table calculations
- Dynamic updates across visuals

---

##  Dashboard Features

- Current temperature display
- 7-day forecast line chart
- Sunrise and Sunset
- City slicer
- Weather KPIs (Humidity, Wind Speed, Pressure, UV Index, Precipitation)
- AQI with color indicators (hazardous, severe, normal, etc.)

---

##  Known Issue

The **"Last Updated" refresh** functionality was previously working correctly but later stopped refreshing dynamically.

Current status:

- City slicer works correctly  
- Forecast and visuals update properly  
- "Last Updated" timestamp does not refresh automatically  

This issue will be investigated and resolved in a future update.

---

##  Dashboard Preview

This dashboard shows real-time weather insights using API data.

<br>

<img width="1333" height="753" alt="Weather Dashboard Preview" src="https://github.com/user-attachments/assets/44be0be7-0f3a-4071-878c-8087b55453f0" />

---

##  Tools Used

- Power BI Desktop
- Power Query
- DAX
- Weather API

---

## 🎯 Learning Outcomes

Through this project, I learned:

- How to connect Power BI with external APIs
- Handling and transforming nested JSON data
- Creating multiple structured tables from a master dataset
- Building relationships for scalable reporting
- Debugging refresh and datatype issues
