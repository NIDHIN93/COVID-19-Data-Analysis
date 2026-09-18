# COVID-19 Data Analysis

## Project Overview

This project performs an exploratory analysis of COVID-19 data using Python and commonly used data analytics libraries.

The analysis examines global COVID-19 trends, country-level reported cases, WHO regional patterns, continental comparisons, and the progression of COVID-19 cases in India.

The project is designed to demonstrate practical skills in data loading, data exploration, aggregation, visualization, and extracting insights from real-world datasets.

> **Data period:** January 22, 2020 – July 27, 2020

---

## Objectives

* Explore and understand COVID-19 datasets.
* Analyze global confirmed cases, deaths, recoveries, and active cases over time.
* Identify countries with the highest reported confirmed case counts.
* Compare COVID-19 statistics across WHO regions.
* Compare reported cases and deaths across continents.
* Analyze the COVID-19 trend in India.
* Create clear visualizations to communicate analytical findings.
* Export analytical summaries and visualizations for further use.

---

## Technologies Used

* **Python**
* **Pandas** — Data manipulation and analysis
* **NumPy** — Numerical operations
* **Matplotlib** — Data visualization
* **Seaborn** — Statistical visualization
* **Jupyter Notebook** — Analysis environment
* **Pathlib** — File and directory management

---

## Datasets

The project uses five COVID-19 datasets.

| Dataset                       |   Rows | Columns | Purpose                                                        |
| ----------------------------- | -----: | ------: | -------------------------------------------------------------- |
| `covid_19_clean_complete.csv` | 49,068 |      10 | Country/province-level COVID-19 records                        |
| `country_wise_latest.csv`     |    187 |      15 | Country-level latest snapshot                                  |
| `day_wise.csv`                |    188 |      12 | Global daily COVID-19 statistics                               |
| `full_grouped.csv`            | 35,156 |      10 | Country-level COVID-19 trends over time                        |
| `worldometer_data.csv`        |    209 |      16 | Country-level cases, deaths, population and testing statistics |

The datasets cover the historical period from **January 22, 2020 to July 27, 2020**.

---

## Analysis Performed

### 1. Data Loading & Exploration

The datasets are loaded using Pandas and inspected using:

* Dataset dimensions
* Column information
* Data types
* Initial records
* Summary statistics

### 2. Top 10 Countries by Confirmed Cases

The country-level dataset is aggregated to identify the countries with the highest reported confirmed case counts.

The results are visualized using a bar chart.

### 3. Global COVID-19 Trend

Daily global totals are analyzed for:

* Confirmed cases
* Deaths
* Recovered cases
* Active cases

A time-series visualization is used to show how these measures changed throughout the dataset period.

### 4. Daily New Cases

Global daily new confirmed cases are analyzed using a time-series chart to identify changes in the reported case trajectory.

### 5. WHO Regional Analysis

COVID-19 statistics are aggregated by WHO region to compare:

* Confirmed cases
* Deaths
* Recovered cases
* Active cases

### 6. Continental Analysis

Worldometer data is grouped by continent to compare reported:

* Total cases
* Total deaths

### 7. India COVID-19 Trend

The country-level time-series data is filtered for India and analyzed over time.

The analysis tracks:

* Confirmed cases
* Deaths
* Recovered cases
* Active cases

---

## Visualizations

The notebook generates the following charts:

* Top 10 countries by reported confirmed cases
* Global COVID-19 totals over time
* Global daily new COVID-19 cases
* Confirmed cases by WHO region
* Cases and deaths by continent
* India's COVID-19 trend

All generated visualizations are saved in the `outputs/` directory.

---

## Project Structure

```text
COVID-19 Data Analysis/
│
├── data/
│   ├── covid_19_clean_complete.csv
│   ├── country_wise_latest.csv
│   ├── day_wise.csv
│   ├── full_grouped.csv
│   └── worldometer_data.csv
│
├── outputs/
│   ├── top_10_confirmed_cases.png
│   ├── global_covid_totals_over_time.png
│   ├── global_daily_new_cases.png
│   ├── confirmed_cases_by_who_region.png
│   ├── cases_and_deaths_by_continent.png
│   ├── india_covid_trend.png
│   ├── beginner_top_10_countries_summary.csv
│   ├── beginner_who_region_summary.csv
│   └── beginner_continent_summary.csv
│
├── COVID19_Data_Analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project directory

```bash
cd COVID-19-Data-Analysis
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
COVID19_Data_Analysis.ipynb
```

### 5. Run the notebook

Run the notebook cells from top to bottom.

The analysis outputs and visualizations will be generated in the `outputs/` directory.

---

## Key Findings

Based on the historical dataset:

* The United States had the highest reported confirmed case count among the countries in the country-level dataset.
* Brazil and India were also among the countries with the highest reported confirmed case counts.
* The Americas recorded the largest aggregate confirmed case count among the WHO regions represented in the dataset.
* North America recorded the largest aggregate total case count among the continents represented in the Worldometer dataset.
* India's reported confirmed cases increased substantially during the analyzed period, reaching **1,480,073** confirmed cases by July 27, 2020.

These findings describe the **reported data contained in the project datasets** and should not be interpreted as estimates of the actual number of infections.

---

## Data Limitations

This project analyzes historical reported COVID-19 data and therefore has important limitations.

* Reported confirmed cases do not necessarily represent the actual number of infections.
* Testing availability and reporting practices varied between countries and over time.
* Differences in case definitions and reporting procedures can affect comparisons.
* Absolute case counts are influenced by population size.
* The analysis covers data only through **July 27, 2020** and does not represent current COVID-19 conditions.

---

## Skills Demonstrated

This project demonstrates practical experience with:

* Python for data analysis
* Pandas DataFrames
* NumPy
* Data exploration
* Data aggregation and grouping
* Time-series analysis
* Country-level analysis
* Regional and continental comparisons
* Matplotlib visualization
* Seaborn visualization
* Exporting analytical results
* Organizing a data analytics project for GitHub

---

## Project Type

**Exploratory Data Analysis (EDA)**

This project focuses on understanding historical COVID-19 data through descriptive analysis and visualization.

---

## Disclaimer

This project is intended for **educational and portfolio purposes**.

The analysis is based on historical datasets and does not provide medical advice, epidemiological forecasting, or current public-health guidance.
