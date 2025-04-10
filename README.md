# 🚕 NYC Yellow Taxi Trip Data Analysis (Jan 2025)

This project analyzes NYC Yellow Taxi trip data from **January 2025**, focusing on time-based patterns, trip durations, and tipping behavior. Built using **PySpark**, it demonstrates how to efficiently handle and transform transportation data using distributed processing tools.

Although the dataset contains only around 50,000 rows—well within the capability of **pandas**—I intentionally chose to implement this project in **PySpark** to strengthen my skills in big data tools and get more hands-on experience with distributed processing techniques.

## 📁 Datasets

- [`yellow_tripdata_2025-01.parquet`](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page): Yellow cab trip records 
- [`taxi-zone-lookup.csv`](https://github.com/EduardTadevosyan/PysparkNYCyellowcab/blob/main/taxi-zone-lookup.xls): Location metadata with zone and borough info

## 🛠 Tech Stack

- Apache Spark (via PySpark)
- Python

## 🔍 Main Features

- Timestamp conversion and duration calculation
- Feature engineering: `pickup_hour`, `day_of_week`, `tip_percent`
- Data cleaning: filter out zero-duration, zero-fare, and invalid distance/passenger entries
- Zone-level insights via joins with location lookup

## 📊 Outcomes

The cleaned and enriched dataset is ready for visual analytics, reporting, and potentially feeding into BI tools like Power BI or real-time dashboards.

## 📓 Notebook

You can view the full code and logic in the following Jupyter Notebook:

👉 [`pyspark.ipynb`](https://github.com/EduardTadevosyan/PysparkNYCyellowcab/blob/main/pyspark.ipynb)

## 🖼 Sample Visual Outputs

Below are some visual summaries from the analysis:

### ⏱️ Average Trip Duration, Distance & Fare by Hour
Hourly breakdown of trips showing how duration, distance, and fare fluctuate across the day.

![Average Trip Data](https://github.com/EduardTadevosyan/PysparkNYCyellowcab/blob/main/Images/The_avg_data.png)

### 📅 Trip Count by Day
Illustrates how the number of daily trips varied throughout the month of January 2025.

![Trip Count by Day](https://github.com/EduardTadevosyan/PysparkNYCyellowcab/blob/main/Images/Total_trips.png)

### 📍 Top 10 Pickup Zones
A ranked summary of the most popular pickup zones across the city during the month.

![Top 10 Pickup Zones](https://github.com/EduardTadevosyan/PysparkNYCyellowcab/blob/main/Images/Top_10_pickup_zones.png)

---

