🚖 Uber NYC Ride Data Analysis (2014–2015)
This project presents a comprehensive analysis of Uber ride data in New York City, leveraging data science techniques to uncover patterns in user behavior, peak demand periods, and geographic ride concentrations. The project applies data wrangling, exploratory data analysis (EDA), time-series breakdown, interactive visualization, and geospatial heat mapping to generate meaningful business insights.

📌 Objective
To perform end-to-end data analysis on Uber’s public NYC datasets from 2014–2015 with the goals of:

Identifying temporal and geographic patterns in ride demand

Visualizing ride density across boroughs and timeframes

Supporting data-driven decisions for marketing, staffing, and logistics

🧰 Tools & Technologies
Category	Tools Used
Programming	Python 3.x
Libraries	pandas, numpy, matplotlib, seaborn, plotly, folium
Data Handling	CSV ingestion, time parsing, missing value handling
Visualization	Bar plots, point plots, box plots, interactive maps
Geospatial Analysis	folium, HeatMap
Environment	Jupyter Notebook, Anaconda, GitHub

📁 Dataset Overview
Datasets are sourced from the NYC Taxi & Limousine Commission and Uber's FOIL release.

uber-raw-data-[apr14–sep14].csv

uber-raw-data-janjune-15_sample.csv

Uber-Jan-Feb-FOIL.csv (Active vehicles & trips by base)

🔍 Key Features & Workflow
1. Data Cleaning & Preprocessing
Removed 82,000+ duplicate records

Converted timestamp strings to datetime objects

Extracted features: Month, Weekday, Hour, Minute

Handled missing values in affiliated base numbers

2. Exploratory Data Analysis
Created pivot tables to compare ride frequency by day & hour

Analyzed ride patterns across different months and weekdays

Used seaborn point plots to reveal hourly demand cycles

Insights generated include:

Highest activity on Thursdays, Fridays, and Saturdays

Peak hour consistently around 11 PM on weekends

3. Uber FOIL Data Analysis
Analyzed active vehicle distribution by base number

Visualized base performance via plotly box plots

Detected patterns in fleet deployment and trip volumes

4. Geospatial Heat Mapping
Grouped ride pickup coordinates (latitude, longitude)

Generated interactive heat maps using folium to highlight high-density areas

Visualized geographic ride intensity to support operational decisions

📊 Sample Insights
Weekend evenings (9 PM–12 AM) show the highest customer demand

Base B02764 recorded the most trips across Jan–Feb 2015

Manhattan and Brooklyn were the dominant ride zones

Data suggests strong opportunities for resource reallocation during peak periods
