# Project-7-Python-For-Data-Analysis-LondonHousing
End-to-end EDA on London Housing data (1995-2019) | Datetime engineering, year/month extraction &amp; crime-price analysis across 45 London areas using Python, Pandas, Matplotlib &amp; Seaborn

# 🏠 Data Analysis Project — London Housing Dataset

An end-to-end Data Analysis project on monthly London housing data spanning 1995–2019, completed as part of the **Python for Data Analysis** course.

## 📌 Objective
Work with real datetime data, engineer year/month features, and answer analytical questions about housing prices, sales volume, and crime trends across 45 London areas.

## 📂 Dataset
- **Source:** LondonHousingData.csv
- **Records:** 13,549 monthly entries
- **Time Range:** January 1995 – September 2019
- **Features:** date, area, average_price, code, houses_sold, no_of_crimes

## 🛠️ Tools & Libraries
| Library | Purpose |
|---|---|
| Pandas | Datetime conversion, feature engineering, filtering, groupby |
| Matplotlib | Time series & base plotting |
| Seaborn | Statistical visualizations, missing values heatmap |

## 🔧 Pandas Commands Covered
| Command | Purpose |
|---|---|
| `pd.to_datetime()` | Convert string column to datetime |
| `.dt.year` / `.dt.month` | Extract year/month from a datetime column |
| `insert()` | Insert a new column at a specific position |
| `drop(axis=1)` | Remove columns permanently |
| `groupby()` | Aggregate data by category |
| `sns.heatmap(df.isnull())` | Visualize missing data |
| Filtering (`df[df.Col == 'X']`) | Extract specific records |

## ❓ Analytical Questions

### Q1 — Convert 'date' column to Date-Time format
Use `pd.to_datetime()` to properly parse the date column.

### Q2 — Add 'year' column, and 'month' as the 2nd column
Extract year and month using `.dt.year` / `.dt.month`, inserting month at position 2 with `insert()`.

### Q3 — Remove the 'year' and 'month' columns
Drop both engineered columns using `drop(axis=1, inplace=True)`.

### Q4 — Records where 'No. of Crimes' is 0
Filter and count all zero-crime records.

### Q5 — Max & Min average_price per year in England
Filter for England, group by year, find max/min average price.

### Q6 — Max & Min No. of Crimes recorded per area
Group by area and aggregate max/min crime counts.

### Q7 — Count of records per area where average_price < 100,000
Filter for affordable housing and count occurrences per area.

## 📊 Analysis Structure
1. Imports & Setup
2. Load Dataset
3. First Look (head / tail)
4. Data Structure & Info
5. Missing Values Check (incl. heatmap)
6. Descriptive Statistics
7. Analytical Questions (Q1 → Q7)
8. Visualizations
   - Univariate (Numerical)
   - Time Series — Price Trend Over Time
   - Bivariate (Num vs Num · Num vs Cat)
   - Correlation Heatmap · Pairplot
9. Key Insights

## 💡 Key Insights
- England's average house price grew dramatically over 24 years, dipping around 2008–2009
- Crime data collection started later than price data (~6,110 missing rows)
- Houses sold and average price show only a weak relationship
- City of London and Inner London dominate the most expensive areas
- Zero-crime months mostly reflect early tracking gaps, not genuinely crime-free periods
- Affordable housing (under £100,000) was almost entirely a 1990s phenomenon

## 🚀 How to Run
```bash
git clone https://github.com/ammarelsayed-2a/Project-7-Python-For-Data-Analysis-LondonHousing.git
cd Project-7-Python-For-Data-Analysis-LondonHousing
jupyter notebook "Project 7 London Housing.ipynb"
```

## 👤 Author
**Ammar Elsayed** — Python for Data Analysis | 2026  
[LinkedIn](https://www.linkedin.com/in/ammar-elsayed-ibrahim)
