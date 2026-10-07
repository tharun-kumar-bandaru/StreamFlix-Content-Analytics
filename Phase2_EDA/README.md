# StreamFlix — Phase 2: Exploratory Data Analysis (EDA)

## Project Overview

StreamFlix is a streaming-platform analytics project designed to analyze subscriber behavior, content consumption, viewing patterns, and customer engagement.

In **Phase 2**, Exploratory Data Analysis (EDA) is performed on the cleaned StreamFlix datasets prepared during Phase 1. The objective is to identify meaningful patterns, trends, distributions, and relationships within subscriber and viewing data.

The analysis focuses primarily on the `watch_history` table and combines it with subscriber, title, and review information to generate business-oriented insights.

---

## Objectives

The main objectives of Phase 2 are to:

- Analyze monthly viewing activity.
- Identify trends in total watch hours.
- Understand genre-wise content consumption.
- Compare Movies and TV Shows.
- Identify the countries contributing the highest watch hours.
- Analyze subscriber plan distribution.
- Understand device usage patterns.
- Analyze the age distribution of subscribers.
- Compare completion rates across genres.
- Analyze review sentiment distribution.
- Generate professional visualizations for business reporting.

---

## Dataset

The StreamFlix project contains six cleaned datasets:

| Dataset | Description |
|---|---|
| `subscribers_cleaned.csv` | Subscriber demographic and subscription information |
| `titles_cleaned.csv` | Movie and TV Show metadata |
| `watch_history_cleaned.csv` | Subscriber viewing activity |
| `ratings_cleaned.csv` | Content ratings provided by subscribers |
| `reviews_cleaned.csv` | Subscriber reviews and sentiment |
| `watchlist_cleaned.csv` | Subscriber watchlist information |

### Approximate Dataset Size

- Subscribers: ~15,000
- Titles: ~9,000
- Watch History: ~650,000
- Ratings: ~130,000
- Reviews: ~110,000
- Watchlist: ~65,000

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## EDA Analysis

Phase 2 contains the following 10 visualizations:

### 1. Monthly Viewing Volume

Analyzes the number of viewing sessions recorded each month and identifies the busiest viewing periods.

**Output:** `01_monthly_viewing_volume.png`

---

### 2. Monthly Watch Hours Trend

Converts viewing duration from minutes into hours and analyzes the monthly trend in total watch time.

**Output:** `02_monthly_watch_hours.png`

---

### 3. Genre-wise Watch Hours

Analyzes total watch hours by content genre to identify the genres receiving the highest viewer engagement.

**Output:** `03_genre_watch_hours.png`

---

### 4. Content Type Split

Compares total watch hours between **Movies** and **TV Shows**.

**Output:** `04_content_type_split.png`

---

### 5. Top 10 Countries by Watch Hours

Identifies the top 10 countries based on total viewing hours.

**Output:** `05_top_10_countries.png`

---

### 6. Subscriber Plan Distribution

Analyzes the distribution of subscribers across different subscription plans.

**Output:** `06_subscriber_plan_distribution.png`

---

### 7. Device Usage

Examines the devices used by subscribers for streaming content.

**Output:** `07_device_usage.png`

---

### 8. Subscriber Age Distribution

Visualizes the age distribution of StreamFlix subscribers.

**Output:** `08_age_distribution.png`

---

### 9. Completion Rate by Genre

Compares the average content completion percentage across different genres.

**Output:** `09_completion_rate_by_genre.png`

---

### 10. Review Sentiment Breakdown

Analyzes the distribution of **Positive, Neutral, and Negative** reviews.

**Output:** `10_review_sentiment_breakdown.png`

---
