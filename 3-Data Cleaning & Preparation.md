# 🧹 Data Cleaning & Preparation

Before conducting the analysis, the dataset underwent a structured **ETL (Extract, Transform, Load)** process using **Microsoft Power Query**. This ensured that the final dataset was accurate, consistent, and suitable for exploratory data analysis.

---

## Cleaning Objectives

The primary objectives of the cleaning process were:

- Improve overall data quality.
- Remove inaccurate or incomplete records.
- Standardize data types.
- Create additional analytical variables.
- Ensure consistency across all twelve monthly datasets.

---

## Data Cleaning Process

The following transformations were applied:

| Task | Description |
|------|-------------|
| Duplicate Removal | Removed duplicated trip records to ensure each ride represented a unique observation. |
| Missing Values | Reviewed missing values in key variables such as `start_station_name` and `end_station_name`. |
| Blank Spaces | Removed unnecessary blank spaces and formatting inconsistencies. |
| Invalid Trips | Removed rides with a duration less than or equal to zero minutes. |
| Date Conversion | Converted date and time fields into the correct DateTime format. |
| Data Type Validation | Verified that every variable contained the appropriate data type. |
| Column Standardization | Renamed columns where necessary to improve readability and consistency. |

---

# 🛠 Feature Engineering

To improve the analysis, several new variables were created from the original dataset.

| New Variable | Description |
|--------------|-------------|
| Ride Length | Duration of each trip |
| Day of Week | Day on which the trip started |
| Month | Month of the trip |
| Season | Winter, Spring, Summer or Fall |
| Hour | Hour when the trip started |

These new variables made it possible to identify behavioral patterns throughout the year and compare riding habits between customer segments.

---

# ✅ Data Validation

Once the cleaning process was completed, several validation checks were performed.

### Validation Checklist

- ✅ Verified all 12 monthly datasets were successfully merged.
- ✅ Confirmed consistent column names across all files.
- ✅ Validated data types.
- ✅ Verified DateTime fields.
- ✅ Confirmed Ride Length calculations.
- ✅ Verified Day of Week extraction.
- ✅ Verified Month extraction.
- ✅ Verified Season classification.
- ✅ Verified Hour extraction.
- ✅ Removed duplicate records.
- ✅ Removed invalid rides.
- ✅ Reviewed missing values.

---

# ⚠️ Data Quality Issues Identified

Several issues were detected before the cleaning process.

| Issue | Resolution |
|--------|------------|
| Duplicate records | Removed |
| Blank values | Reviewed and cleaned |
| Missing station names | Evaluated and retained when appropriate |
| Incorrect data types | Converted |
| Negative ride durations | Removed |
| Inconsistent formatting | Standardized |

Overall, the dataset presented good quality after applying the ETL process.

---

# 📈 Exploratory Data Analysis (EDA)

After preparing the dataset, an exploratory analysis was conducted to better understand customer behavior.

The objective was to identify differences between **Annual Members** and **Casual Riders** through descriptive statistics and visual analysis.

---

# 📊 Key Performance Indicators (KPIs)

The following KPIs were calculated during the analysis.

| KPI | Description |
|------|-------------|
| Total Trips | Total rides completed by each customer type |
| Average Ride Duration | Average trip duration |
| Trips by Rider Type | Distribution of Members vs Casual Riders |
| Trips by Day of Week | Weekly riding behavior |
| Trips by Month | Monthly demand |
| Trips by Season | Seasonal demand |
| Trips by Hour | Hourly usage patterns |
| Bike Type Usage | Preferred bicycle type |
| Top 10 Stations | Most frequently used stations |

---

# 📐 Metrics Calculation

The KPIs were calculated using the following methodology.

| Metric | Calculation |
|---------|-------------|
| Total Trips | Count of `started_at` |
| Average Ride Duration | Average of `ride_length` |
| Trips by Rider Type | Count grouped by `member_casual` |
| Trips by Month | Count grouped by `month` |
| Trips by Season | Count grouped by `season` |
| Trips by Hour | Count grouped by `hour` |
| Bike Type Usage | Count grouped by `rideable_type` |
| Top Stations | Count grouped by `start_station_name` |

---

# 🔍 Initial Observations

Before creating visualizations, several patterns were immediately noticeable.

- Twelve months of historical data were available.
- The dataset contained two distinct customer segments.
- Multiple bicycle types were available.
- Ride activity covered all seasons.
- Trip records included origin and destination stations.
- Data quality issues required preprocessing before analysis.

These observations guided the exploratory analysis and helped define the hypotheses.

---

# 💡 Initial Hypotheses

Based on the initial review of the dataset, three hypotheses were established.

## Hypothesis 1

Annual Members complete more trips throughout the year, while Casual Riders tend to have longer average ride durations.

---

## Hypothesis 2

Casual Riders increase their activity significantly during the summer months, whereas Members maintain a more consistent riding pattern throughout the year.

---

## Hypothesis 3

Members primarily use Cyclistic bicycles for commuting, resulting in peak activity during morning and afternoon rush hours.

Casual Riders, on the other hand, are expected to ride more evenly throughout the day due to recreational use.

---

# 📊 Dashboard Overview

A business dashboard was created to compare the behavior of Annual Members and Casual Riders.

The dashboard includes:

- Average Ride Duration
- Trips by Rider Type
- Trips by Day of Week
- Trips by Month
- Trips by Season
- Trips by Hour
- Bike Type Preference
- Top 10 Most Used Stations

The visualizations provide a comprehensive overview of customer behavior and support data-driven business recommendations.

---
