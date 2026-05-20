# 📊 E-Commerce Sales Analytics using Pandas & Matplotlib

This project performs **Exploratory Data Analysis (EDA)** and **Data Visualization** on an E-Commerce Sales dataset using Python.

We use:

- **Pandas** → Data manipulation & analysis  
- **Matplotlib** → Data visualization  

---

## 📌 Project Objectives

The goal of this project is to analyze e-commerce sales data and extract insights such as:

- Monthly revenue trends
- Customer behavior patterns
- Product category performance
- Payment method distribution
- Delivery performance
- Discount impact on revenue

---

## 📂 Dataset Loading

We load the dataset using Pandas and convert the `order_date` column into datetime format for time-series analysis.

```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv(
    "ecommerce_sales_analytics_5000.csv",
    parse_dates=["order_date"]
)

df.head()
df.shape
````

### 🔍 Why `parse_dates`?

* Converts `order_date` into datetime format
* Enables resampling and time-series analysis

---

## 📈 Monthly Revenue Trend

We analyze total monthly revenue using time-series resampling.

```python
monthly_revenue = (
    df.set_index("order_date")["revenue"]
    .resample("ME")
    .sum()
)
```

### Key Concepts:

* `set_index()` → Set date column for time-series
* `resample("ME")` → Monthly grouping
* `sum()` → Total revenue per month

---

## 🔍 Unit Price vs Revenue (Scatter Plot)

Shows relationship between product price and revenue.

### Insights:

* Detect correlation
* Identify outliers
* Understand pricing impact

---

## 💳 Payment Method Analysis

We analyze how customers prefer to pay.

```python
df["payment_method"].value_counts()
```

### Insights:

* Most used payment methods
* Customer payment behavior

---

## 📊 Product Category Analysis

### Total Revenue by Category

```python
df.groupby("product_category")["revenue"].sum()
```

### Mean & Variability

```python
df.groupby("product_category")["revenue"].agg(["mean", "std"])
```

### Insights:

* Best performing categories
* Revenue consistency per category

---

## 🌍 Revenue by Category & Region

We analyze revenue distribution across regions.

### Techniques Used:

* `groupby()`
* `unstack()`
* Grouped bar charts
* Stacked bar charts

### Insights:

* Regional performance differences
* Category-wise dominance per region

---

## 📊 Delivery Time & Customer Ratings

We visualize:

* Delivery time distribution
* Customer rating distribution

### Insights:

* Delivery efficiency
* Customer satisfaction trends

---

## 📉 Revenue Distribution Analysis

We compare:

* Original revenue distribution
* Discounted revenue impact

```python
discounted_revenue = df["revenue"] * (1 - df["discount"])
```

### Insights:

* Effect of discounts on revenue
* Revenue spread and density

---

## 📉 Monthly Revenue Confidence Band

We calculate:

* Mean revenue
* Standard deviation
* Confidence interval visualization

```python
monthly = (
    df.set_index("order_date")["revenue"]
    .resample("ME")
    .agg(["mean", "std"])
)
```

### Insights:

* Revenue stability over time
* Seasonal variations

---

## 📦 Tools & Libraries Used

* Python 🐍
* Pandas 📊
* Matplotlib 📈

---

## 🚀 Key Learnings

* Time-series analysis using Pandas
* Data aggregation and grouping
* Data visualization techniques
* Business insight extraction from raw data

---

## 📌 Output

All plots generated include:

* Line charts
* Scatter plots
* Bar charts
* Histograms
* Stacked & grouped charts
* Confidence band visualization

---

## ⭐ Author

Fatima Ijaz
