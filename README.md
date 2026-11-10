# Kagnus Food Delivery Data Analysis
Junior data analyst operations project investigating delivery duration patterns across traffic, weather, distance, and vehicle types.

## Project Structure
- `data/raw/`: Original dataset (`Food delivery Dataset.csv`)
- `data/processed/`: Cleaned dataset (`cleaned_food_delivery.csv`)
- `notebooks/`: Jupyter notebooks for data cleaning and EDA
- `docs/`: Cleaning logs and documentation# Kagnus Food Delivery Data Analysis

## Project Overview
As a junior data analyst supporting the food-delivery operations team, this project investigates raw delivery records to uncover evidence-based operational insights across traffic density, weather conditions, delivery distance, vehicle types, and partner demographics[cite: 1, 2].

## Repository Structure
food-delivery-data-analysis/
├── data/
│   ├── raw/
│   │   └── README.md
│   └── processed/
│       └── cleaned_food_delivery.csv
├── notebooks/
│   └── 01_data_understanding_and_cleaning.ipynb
├── docs/
│   └── cleaning_log.csv
├── README.md
└── requirements.txt

## Tools & Libraries
* **Python 3.13**
* **Pandas & NumPy** (Data inspection, cleaning, and Haversine distance calculations)
* **Matplotlib & Seaborn** (Visual quality checks)
* **Jupyter Notebook / VS Code**

## Instructions to Run
1. Clone the repository and open it in VS Code or Jupyter Notebook.
2. Ensure required packages are installed by running: `pip install -r requirements.txt`
3. Open `notebooks/01_data_understanding_and_cleaning.ipynb` and run all cells sequentially from top to bottom.

## Week 1 Summary & Observations
* **Initial Profile:** Loaded 45,584 raw delivery records across 20 operational columns.
* **Data Quality Actions:** Addressed missing values via median and categorical mode/unknown imputations, filtered out 4,071 coordinate outliers falling outside Indian geographic boundaries, and engineered the direct `Distance_km` feature using the Haversine formula.
* **Cleaned Output:** Finalized dataset contains 41,513 reliable rows stored in `data/processed/cleaned_food_delivery.csv`.

## Week 2: Exploratory Data Analysis (EDA)
* **Delivery Baseline:** Evaluated distribution metrics across 41,513 valid records (mean duration: 26.31 minutes, median: 26.0 minutes).
* **Operational Comparisons:** Compiled comparative summary tables for road traffic density, weather conditions, and vehicle categories.
* **Distance Analysis:** Calculated correlation and exported the initial distance-versus-duration scatter plot to `visualizations/initial_distance_vs_duration.png`.
* **Key Observations:** Documented five number-supported operational insights.