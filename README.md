# COVID-19 Data Analysis and Visualization

This project performs data preprocessing and visualizations on a COVID-19 dataset using **Pandas**, **Seaborn**, and **Matplotlib**.

The dataset is sourced from Kaggle and includes COVID-19 statistics like total cases, deaths, discharges, and population.

## 📁 Dataset
- File: `covid.csv`
- Source: [Kaggle](https://www.kaggle.com/)
- Required columns:
  - `State`
  - `Total Cases`
  - `Active`
  - `Discharged`
  - `Deaths`
  - `Population (millions)`

---

## ✅ Steps Performed

### 1. 📊 Data Cleaning and Feature Engineering
- Removed extra spaces in column names
- Created new computed columns:
  - `Active Ratio` = (`Active` / `Total Cases`) * 100
  - `Discharge Ratio` = (`Discharged` / `Total Cases`) * 100
  - `Death Ratio` = (`Deaths` / `Total Cases`) * 100
  - `Cases per Million` = `Total Cases` / `Population (millions)`

### 2. 📈 Data Visualizations (Seaborn & Matplotlib)
- **Bar Plot** – Death Ratio by State
- **Pie Chart** – Top 5 States by Total Cases
- **Scatter Plot** – Total Cases vs Deaths (colored by State)
- **Heatmap** – Correlation between numerical features

---

## 📌 Requirements

```bash
pip install pandas seaborn matplotlib
