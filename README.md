# 🚖 Uber NYC Ride Data Analysis (2014–2015)

This project analyzes Uber ride data in New York City using data science techniques to identify trends in ride volume, peak hours, and geographic hot spots. The goal is to uncover insights that can inform operations, marketing, and urban planning.

---

## 📌 Objective

Analyze Uber’s public ride datasets from 2014–2015 to:

- Identify **temporal and geographic patterns** in ride demand  
- Visualize ride density and behavior across boroughs and times  
- Provide **actionable insights** to optimize business decisions

---

## 🧰 Tools & Technologies

| Category           | Tools Used                                               |
|--------------------|----------------------------------------------------------|
| Programming        | Python 3.x                                               |
| Libraries          | `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `folium` |
| Visualization      | Bar charts, Point plots, Box plots, Heatmaps             |
| Geospatial Mapping | `folium`, `HeatMap` plugin                               |
| Environment        | Jupyter Notebook, Anaconda, GitHub                       |

---

## 📁 Dataset Overview

| Dataset Name                              | Description                                  |
|------------------------------------------|----------------------------------------------|
| `uber-raw-data-[apr14–sep14].csv`        | Monthly raw trip data                        |
| `uber-raw-data-janjune-15_sample.csv`    | Sample Uber trip data (Jan–June 2015)        |
| `Uber-Jan-Feb-FOIL.csv`                  | Base-level active vehicle & trip info        |

---

## 🔍 Key Features & Workflow

### 🧹 1. Data Cleaning
- Removed **82,000+ duplicates**
- Converted timestamp strings to `datetime`
- Extracted time features: `Month`, `Weekday`, `Hour`, `Minute`
- Addressed missing values in base number fields

### 📊 2. Exploratory Data Analysis (EDA)
- Created pivot tables by **weekday and hour**
- Visualized hourly ride patterns with `seaborn.pointplot`
- Generated monthly trends using `pandas` and `matplotlib`

✅ Insights:
- High demand on **Thursdays, Fridays, and Saturdays**
- Peak hours between **9 PM – 12 AM**, especially on weekends

### 📦 3. Uber FOIL Data Exploration
- Analyzed active vehicle and trip volume by dispatch base
- Visualized base activity using interactive `plotly.box`

### 🌍 4. Geospatial Heatmaps
- Aggregated latitude/longitude pairs to count ride density
- Used `folium` + `HeatMap` to generate interactive NYC heatmaps

---

## 📊 Sample Insights

- **Saturday 11 PM** is peak ride time — target for promos/staffing  
- **Base B02764** had highest trip count in early 2015  
- **Manhattan & Brooklyn** were high-density ride zones
