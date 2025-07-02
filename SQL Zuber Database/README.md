# SQL Zuber Database Analysis

![image alt](https://github.com/ejcuison/TripleTen-Projects/blob/4eb94085bd113fb6696b6fbaa4b1b5492b89d966/SQL%20Zuber%20Database/Query%202.png)

## Project Overview

This project explores ride and weather data from the **Zuber** database using SQL. The analysis focuses on taxi ride patterns in November 2017, comparing company performance, evaluating weather impact on trip durations, and filtering specific trip routes by conditions.

## Tools Used

- SQL

## Data Source

- Zuber Database

## Objectives

1. Analyze taxi rides by company during specific date ranges.
2. Filter and group companies by name patterns (e.g., containing "Blue" or "Yellow").
3. Compare top-performing taxi companies against all others.
4. Identify neighborhood IDs for targeted ride filtering.
5. Categorize weather conditions hourly and assess impact on trip durations.
6. Match trips between Loop and O’Hare on Saturdays with weather data.

## Queries Summary

### 📊 Query 1
Counted rides per company for **Nov 15–16, 2017**.  
- Output: `company_name`, `trips_amount`  
- Sorted by `trips_amount` descending.

### 🔍 Query 2
Counted rides from companies containing **"Yellow" or "Blue"** in their names for **Nov 1–7, 2017**.  
- Output grouped by `company_name`.

### 🏆 Query 3
Compared **Flash Cab** and **Taxi Affiliation Services** to all others (grouped as "Other") for **Nov 1–7, 2017**.  
- Output: `company`, `trips_amount`  
- Sorted by `trips_amount` descending.

### 📍 Query 4
Retrieved neighborhood IDs:  
- **Loop**: `50`  
- **O'Hare**: `63`

### ☁️ Query 5
Classified hourly weather as **"Good"** or **"Bad"** using the `description` field in `weather_records`.  
- Conditions: "rain" or "storm" → "Bad", others → "Good"  
- Output: `date`, `ts` (hour), `weather_conditions`

### 🚖 Query 6
Retrieved rides on **Saturdays** from **Loop (50)** to **O’Hare (63)**, matched with weather data.  
- Output included: `duration`, `weather_conditions`  
- Excluded rides without weather info.

## Results & Insights

- **Top 3 companies** (Nov 15–16, 2017):
  - Flash Cab: **19,558 rides**
  - Taxi Affiliation Services: **11,422 rides**
  - Medallion Leasing: **10,367 rides**

- **"Blue"/"Yellow" companies** (Nov 1–7, 2017):
  - Yellow Cab: **33,668**
  - Taxi Affiliation Service Yellow: **29,213**
  - Blue Ribbon Taxi Association: **17,675**
  - Blue Diamond: **6,764**

- **Top 2 companies vs. Others** (Nov 1–7, 2017):
  - Flash Cab: **64,084**
  - Taxi Affiliation Services: **37,583**

- **Neighborhood IDs**:
  - Loop: `50`
  - O’Hare: `63`

- **Weather overview** (Nov 1–9, 2017):
  - Mostly **Good**
  - **Bad weather** on: Nov 2, 4, 5, 7

- **Trip durations** (Loop → O’Hare, Saturdays):
  - Trips in **Bad weather** were **slightly longer** than in Good weather.

## Conclusion

This project highlights how SQL can be used to derive actionable insights from urban mobility data, revealing patterns across companies, dates, weather, and geographic zones.

