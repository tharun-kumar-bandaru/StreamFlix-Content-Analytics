# StreamFlix — Phase 1: Data Cleaning & Quality Check

## Project Overview

StreamFlix is a Content Analytics project focused on understanding subscriber activity, content performance, viewing behaviour, and data quality.

Phase 1 focuses on **loading, cleaning, validating, and profiling the StreamFlix dataset** before performing Exploratory Data Analysis (EDA).

The project contains six interconnected datasets with approximately **979,000 records** covering subscriber and viewing activity across multiple years. :chatgpt-content-reference{index="0"}

---

## Objectives

The main objectives of Phase 1 are:

- Load all six CSV datasets.
- Understand the structure and size of each dataset.
- Check data types.
- Identify missing values.
- Detect duplicate records.
- Validate important IDs.
- Check data quality and business rules.
- Verify relationships between tables.
- Identify potential outliers.
- Prepare clean and reliable datasets for Phase 2.

---

## Datasets

| Dataset | Description |
|---|---|
| `subscribers.csv` | Subscriber profiles, plans, location, tenure and churn information |
| `titles.csv` | Content catalogue, genres, languages, licensing and popularity |
| `watch_history.csv` | Viewing sessions and engagement information |
| `ratings.csv` | Subscriber ratings for titles |
| `reviews.csv` | Written reviews, sentiment and helpful votes |
| `watchlist.csv` | Titles saved by subscribers and whether they were watched |

The `watch_history.csv` file is the central fact table containing approximately **650,000 viewing sessions**. :chatgpt-content-reference{index="1"}

---

## Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Data Quality Checks

### 1. Dataset Profiling

For each dataset, the following were checked:

- Number of rows
- Number of columns
- Column names
- Data types
- Sample records

### 2. Missing Value Analysis

Missing values were checked for every column and their percentage was calculated.

### 3. Duplicate Analysis

Duplicate records were checked across all datasets.

Special checks were performed for:

- `subscriber_id`
- `watch_id`

### 4. Data Type Validation

Important fields were validated and converted where necessary.

Examples:

- `watch_date`
- `signup_date`
- `churn_date`
- `watch_duration_min`
- `completion_pct`
- `monthly_price_usd`
- `license_cost_usd`

### 5. Referential Integrity

Relationships between datasets were validated.

Examples:

```text
watch_history.subscriber_id
        ↓
subscribers.subscriber_id
