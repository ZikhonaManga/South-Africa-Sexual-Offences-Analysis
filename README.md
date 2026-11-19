# Mapping Sexual Offence Trends in South Africa (2015/16–2024/25)

## 1. Project Overview

This project analyses reported rape cases across South Africa using South African Police Service (SAPS) crime statistics covering the 2015/16 to 2024/25 financial years.

The objective is to explore national trends, compare provincial figures and investigate police station-level patterns to identify changes in reported rape cases over time.

Python was used for data cleaning, exploratory data analysis (EDA), statistical comparisons and data visualisation.

## 2. Project Objectives

- Analyse national reported rape trends over ten financial years.
- Compare reported rape cases across South Africa's nine provinces.
- Calculate absolute and percentage changes between 2015/16 and 2024/25.
- Identify the ten police stations with the highest reported rape cases in 2024/25.
- Examine historical trends among the selected police stations.
- Communicate findings through data visualisations.

## 3. Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and programming |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Jupyter Notebook | Analysis and documentation |
| Excel | Initial dataset inspection |

## 4. Dataset Description

**Source:** South African Police Service (SAPS) crime statistics.

**Period:** 2015/16–2024/25.

**Geographical coverage:** South Africa, including all nine provinces and individual police stations.

The original dataset was supplied in Excel format and contained crime statistics at different aggregation levels, including national, provincial, district and police station records.

The analysis specifically focuses on the crime category **Rape**.

## 5. Data Cleaning and Preparation

The following preparation steps were performed:

1. Imported the Excel dataset into Python using Pandas.
2. Inspected the dataset structure, column names and missing values.
3. Identified non-data rows containing report headings.
4. Removed rows without a valid crime category.
5. Checked for duplicate records.
6. Filtered the cleaned dataset to focus on reported rape cases.
7. Separated national, provincial and police station records using the `Comp level` column to prevent double-counting aggregated figures.

After cleaning, the dataset contained **48,243 rows and 25 columns**, with no missing values or duplicate rows.

## 6. Exploratory Data Analysis and Visualisations

### 6.1 National Rape Trends

The national analysis examined reported rape cases over ten financial years.

![National Rape Trends](visualisation/national_rape_trend.png)

### 6.2 Provincial Comparison (2024/25)

Compared reported rape cases across South Africa's nine provinces for the latest financial year in the dataset.

![Provincial Comparison](visualisation/provincial_comparison_2024_25.png)

### 6.3 Provincial Percentage Changes

Calculated the percentage change in reported rape cases between 2015/16 and 2024/25 for each province.

![Provincial Percentage Changes](visualisation/provincial_percentage_change.png)

### 6.4 Provincial Trends Over Time

Examined how reported rape cases changed across the nine provinces over the ten-year period.

![Provincial Trends Over Time](visualisation/provincial_trends_over_time.png)

### 6.5 Top 10 Police Stations (2024/25)

Identified the ten police stations with the highest reported rape case counts in 2024/25.

![Top 10 Police Stations](visualisation/top10_police_stations_2024_25.png)

### 6.6 Trends Among the Top 10 Police Stations

Compared historical reported rape case counts among the ten stations selected using their 2024/25 figures.

![Top 10 Station Trends](visualisation/top10_station_trends.png)

## 7. Key Findings

### National Findings

- The highest national figure was recorded in 2022/23, with 42,780 reported cases.
- The lowest figure was recorded in 2020/21, with 36,330 reported cases.
- In 2024/25, 40,475 rape cases were reported.

### Provincial Findings

- Gauteng recorded the highest number of reported rape cases in 2024/25, with 8,200.
- KwaZulu-Natal followed with 7,855 cases.
- The Eastern Cape recorded 6,325 cases.
- The Northern Cape recorded the lowest figure, with 1,045 cases.
- Gauteng experienced the largest percentage increase between 2015/16 and 2024/25, at 7.82%.
- The Northern Cape recorded the largest percentage decrease, at 18.80%.
- The Eastern Cape recorded the largest absolute decrease, with 1,112 fewer reported cases.

### Police Station Findings

The ten police stations with the highest reported rape cases in 2024/25 were:

| Rank | Police Station | Province | Reported Cases |
|---|---|---|---:|
| 1 | Inanda | KwaZulu-Natal | 302 |
| 2 | Thohoyandou | Limpopo | 272 |
| 3 | Lusikisiki | Eastern Cape | 252 |
| 4 | Umlazi | KwaZulu-Natal | 251 |
| 5 | Mthatha | Eastern Cape | 244 |
| 6 | Mfuleni | Western Cape | 225 |
| 7 | Roodepoort | Gauteng | 201 |
| 8 | Plessislaer | KwaZulu-Natal | 200 |
| 9 | Bloemspruit | Free State | 196 |
| 10 | Mountain Rise | KwaZulu-Natal | 189 |

Among these ten stations:

- Roodepoort recorded the largest percentage increase between 2015/16 and 2024/25, at 151.25%.
- Lusikisiki recorded the second-largest increase, at 82.61%.
- Umlazi and Plessislaer were the only two stations in this group to record decreases.

## 8. Methodology

The project followed a data analysis workflow:

1. Data collection and initial inspection.
2. Data cleaning and preparation.
3. Filtering and extraction of relevant crime records.
4. Aggregation and comparison at national, provincial and police station levels.
5. Exploratory data analysis.
6. Calculation of absolute and percentage changes.
7. Data visualisation.
8. Interpretation and documentation of findings.

## 9. Limitations

- The dataset represents reported rape cases and does not capture all incidents that may have occurred.
- Reported case counts should not be interpreted as the actual prevalence of rape.
- The analysis uses raw counts rather than population-adjusted rates.
- Changes in reported cases do not necessarily indicate changes in the actual occurrence of rape.
- The analysis does not establish the causes behind observed increases or decreases.
- The police stations selected for historical comparison were chosen based on their 2024/25 reported case counts and do not represent all stations with increasing trends.

## 10. Conclusion

This project demonstrates how Python can be used to clean, analyse and visualise real-world crime statistics.

The analysis identified national, provincial and police station-level patterns in reported rape cases across South Africa between 2015/16 and 2024/25.

The findings highlight differences in reported case counts across geographical areas and changes over time. They also demonstrate the importance of interpreting crime statistics carefully, considering reporting limitations and distinguishing raw counts from population-adjusted measures.

Overall, the project provided practical experience in data cleaning, exploratory data analysis, numerical comparisons and communicating insights through visualisations.

## 11. Project Structure

```text
South-Africa-Sexual-Offences-Analysis/
│
├── README.md
│
├── data/
│   ├── raw/
│   │   └── SAPS_RAW_Data_Working_Copy.xlsx
│   │
│   └── cleaned/
│       └── saps_cleaned.csv
│
├── notebooks/
│   └── 01_data_cleaning.ipynb
│
└── visualisation/
    ├── national_rape_trend.png
    ├── provincial_comparison_2024_25.png
    ├── provincial_percentage_change.png
    ├── provincial_trends_over_time.png
    ├── top10_police_stations_2024_25.png
    └── top10_station_trends.png
```

## 12. How to Run This Project

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib openpyxl jupyter
```

4. Open the project directory.
5. Launch Jupyter Notebook.
6. Open `notebooks/01_data_cleaning.ipynb`.
7. Run the notebook cells in sequence.

---

**Project Focus:** Data Analytics | Exploratory Data Analysis | Python | Data Visualisation

**Dataset:** South African Police Service (SAPS) Crime Statistics