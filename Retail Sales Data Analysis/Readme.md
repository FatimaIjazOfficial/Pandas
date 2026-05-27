# 📊 Retail Sales Data Analysis

A complete **Retail Sales Data Analysis Project** using **Python, Pandas, NumPy, Seaborn, and Matplotlib**.
This project demonstrates a full **data analysis workflow** including:

* Data Cleaning
* Data Transformation
* Feature Engineering
* Missing Value Handling
* Exploratory Data Analysis (EDA)
* Data Visualization
* Statistical Analysis
* Exporting Processed Data

---

# 🚀 Project Overview

The goal of this project is to analyze retail sales data and extract meaningful business insights such as:

* Monthly sales trends
* Profit analysis
* Regional performance
* Category-wise sales
* Day-of-week performance
* Correlation between numerical variables
* Profitability analysis

---

# 🛠️ Technologies & Libraries Used

| Library    | Purpose                        |
| ---------- | ------------------------------ |
| Pandas     | Data manipulation and analysis |
| NumPy      | Numerical computations         |
| Matplotlib | Data visualization             |
| Seaborn    | Statistical visualization      |

---

# 📂 Dataset Features

The dataset contains retail sales information such as:

* Date
* Category
* Region
* Sales
* Quantity
* Profit

---

#  Project Workflow

## 1️⃣ Importing Libraries

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

---

## 2️⃣ Data Loading

```python
df = pd.read_csv('retail_sales.csv')
```

---

## 3️⃣ Data Cleaning

Performed several preprocessing steps:

* Converted date columns into datetime format
* Optimized categorical columns
* Converted numeric columns safely
* Handled missing values
* Removed invalid records
* Checked duplicates

---

## 4️⃣ Feature Engineering

Created additional features such as:

| Feature   | Description      |
| --------- | ---------------- |
| Month     | Month number     |
| Quarter   | Business quarter |
| DayOfWeek | Weekday name     |
| MonthName | Full month name  |

---

## 5️⃣ Exploratory Data Analysis (EDA)

Performed:

* Descriptive statistics
* Sorting & ranking
* Correlation analysis
* GroupBy aggregations

---

# 📈 Visualizations

The project includes several visualizations:

## 📅 Monthly Sales & Profit Trend

* Line plot for monthly sales and profit analysis

## 📊 Category-wise Sales Analysis

* Bar chart for product category performance

## 🌍 Regional Sales Distribution

* Pie chart showing regional contribution

## 🔥 Correlation Heatmap

* Heatmap showing relationships between:

  * Sales
  * Quantity
  * Profit

---

# 📉 Profitability Analysis

Calculated:

* Overall profit margin
* Category-wise profit margins
* Best performing region
* Best sales month
* Best sales day

---

# 💾 Exporting Processed Data

Exported cleaned datasets into:

## Excel Format

```python
subset.to_excel("subset_sales.xlsx", index=False)
```

## JSON Format

```python
subset.to_json(
    "subset_sales.json",
    orient="records",
    date_format="iso"
)
```

---

# 📊 Key Insights

✔ Highest performing category identified
✔ Best performing region analyzed
✔ Monthly sales trends discovered
✔ Day-wise sales behavior analyzed
✔ Correlation between sales and profit evaluated

---

# ▶️ How to Run the Project

## Clone Repository

```bash
git clone https://github.com/your-username/Retail-Sales-Analysis.git
```

## Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

## Run Jupyter Notebook

```bash
jupyter notebook
```

---

# 📌 Future Improvements

* Add dashboard using Streamlit or Power BI
* Add predictive sales forecasting
* Add customer segmentation
* Perform advanced statistical analysis
* Add interactive visualizations

---

# 🤝 Contributing

Contributions are welcome!
Feel free to fork the repository and submit pull requests.

---

# ⭐ If You Like This Project

Give this repository a ⭐ on GitHub to support the project!
