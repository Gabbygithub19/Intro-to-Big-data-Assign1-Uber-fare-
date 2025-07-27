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

## How to Use

1. **Run the Notebook:**  
   Open `uber-fare-data-analysis.ipynb` in Jupyter or VS Code and execute cells sequentially.
2. **Review Outputs:**  
   Inspect data cleaning, EDA, and feature engineering results.
3. **Exported Files:**  
   Use `uber_cleaned.csv` or `uber_enhanced.csv` for Power BI analysis.
4. **Power BI:**  
   Import the exported CSV into Power BI Desktop to build interactive dashboards.

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

## License

This project is for educational purposes. The Uber dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/fivethirtyeight/uber-pickups-in-new-york-city)
