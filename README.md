# Uber Fare Data Analysis

This project analyzes Uber ride fare data to uncover patterns, trends, and operational insights. The workflow includes data cleaning, exploratory data analysis (EDA), feature engineering, and exporting datasets for interactive visualization in Power BI.

---

## Project Structure

```
assignment-uber/
│
├── uber.csv                      # Raw Uber fares dataset (from Kaggle)
├── uber_cleaned.csv              # Cleaned dataset (ready for Power BI)
├── uber_enhanced.csv             # Enhanced dataset with engineered features
├── uber-fare-data-analysis.ipynb # Jupyter Notebook with all analysis steps
└── README.md                     # Project documentation (this file)
```

---

## Workflow Overview

### 1. Data Understanding and Preparation
- **Load Data:** Import the raw Uber fares dataset (`uber.csv`) into a Pandas DataFrame.
- **Explore Structure:** Review dataset dimensions, data types, and variable descriptions.
- **Initial Assessment:** Check for missing values and data quality issues.

### 2. Data Cleaning
- **Remove Invalid Rows:** Drop rows with missing values, zero coordinates, negative/zero fares, or invalid passenger counts.
- **Export Cleaned Data:** Save as `uber_cleaned.csv` for use in Power BI.

### 3. Exploratory Data Analysis (EDA)
- **Descriptive Statistics:** Calculate mean, median, mode, standard deviation, quartiles, and identify outliers.
- **Visualizations:** Plot fare distributions, fare vs. distance, fare vs. time of day, and correlation heatmaps.

### 4. Feature Engineering
- **Time Features:** Extract hour, day, month, and day of week from pickup timestamps.
- **Peak/Off-Peak:** Create a categorical feature indicating peak and off-peak ride times.
- **Export Enhanced Data:** Save as `uber_enhanced.csv` for advanced analysis in Power BI.

### 5. Power BI Dashboard (External)
- **Import Data:** Load `uber_cleaned.csv` or `uber_enhanced.csv` into Power BI Desktop.
- **Create Visuals:** Analyze fare patterns, ride frequency, time trends, and highlight busiest periods.

---

## Deliverables

- **Cleaned Datasets:**  
  - `uber_cleaned.csv`: Cleaned data for analysis and Power BI import  
  - `uber_enhanced.csv`: Data with additional engineered features

- **Screenshots:**  
-- **Output 1**
<img width="876" height="547" alt="output1" src="https://github.com/user-attachments/assets/84b251e7-24f0-471a-a63e-562f1a5cdf5e" />
-- **Output 2**
<img width="850" height="547" alt="output2" src="https://github.com/user-attachments/assets/f6aedd91-aeaf-4c49-a402-8179519b06c7" />
-- **Output 3**
<img width="1005" height="547" alt="output3" src="https://github.com/user-attachments/assets/646bba29-1dfb-459b-8602-46133a6deed6" />
-- **Output 4**
<img width="625" height="528" alt="output4" src="https://github.com/user-attachments/assets/bb1b96e0-de0d-4eba-baf4-61015260ae60" />

---

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- Jupyter Notebook or VS Code

---

## Dataset Fields

- `key`: Unique trip identifier
- `fare_amount`: Fare paid (USD)
- `pickup_datetime`: Pickup date and time
- `pickup_longitude`, `pickup_latitude`: Pickup coordinates
- `dropoff_longitude`, `dropoff_latitude`: Dropoff coordinates
- `passenger_count`: Number of passengers
- *(Enhanced features: `hour`, `day`, `month`, `day_of_week`, `peak_offpeak`)*

---
