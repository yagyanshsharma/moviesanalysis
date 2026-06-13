# 🎬 Movie Analysis Project

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Latest-purple.svg)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Latest-orange.svg)](https://matplotlib.org/)

An end-to-end data analysis project exploring a massive dataset of **9,999 movies and TV shows**. This project focuses on data cleaning, parsing complex text formats, extracting insights, and visualizing trends across genres, ratings, and release years.

---

## 📌 Project Overview
The entertainment industry produces thousands of titles yearly, but what makes a movie or show truly successful? This notebook ingests raw data (`movies.csv`) containing structural inconsistencies, missing values (`NaN`), and messy strings to uncover meaningful patterns in audience preferences, runtimes, and ratings.

### Key Focus Areas:
* **Data Cleaning & Polishing:** Stripping raw newline characters (`\n`), handling missing values in ratings/gross metrics, and splitting compound strings (like `STARS` and `GENRE`).
* **Exploratory Data Analysis (EDA):** Dissecting distribution curves for movie ratings and identifying dominant genre combinations.
* **Trend Analysis:** Monitoring how runtimes and audience engagement have evolved over time.

---

## 📊 Dataset Structure
The raw dataset consists of **9,999 rows** and **9 columns**:

| Column Name | Description | Data Status (Raw) |
| :--- | :--- | :--- |
| `MOVIES` | Title of the movie / TV show | Clean text |
| `YEAR` | Release year or active broadcasting span | Contains brackets and ranges (e.g., `(2010–2022)`) |
| `GENRE` | Associated entertainment genres | Prefixed with `\n` and comma-separated strings |
| `RATING` | IMDb / User rating out of 10 | Numeric (contains missing values) |
| `ONE-LINE` | Brief synopsis of the plot | Prefixed with `\n` |
| `STARS` | Director and main cast information | Messy string mixing Directors and Stars |
| `VOTES` | Number of user reviews | Object type with commas (e.g., `21,062`) |
| `RunTime` | Duration of the title in minutes | Float format |
| `Gross` | Total box office earnings | Highly sparse (contains significant `NaN`) |

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib.pyplot`
* **Environment:** JupyterLab / Jupyter Notebook

---

## 🚀 Getting Started

### 1. Prerequisites
Ensure you have Python installed, then install the required dependencies:
```bash
pip install pandas numpy matplotlib
