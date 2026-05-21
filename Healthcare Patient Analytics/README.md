# 🏥 Healthcare Patient Analytics

## 📌 Overview

This project performs **Exploratory Data Analysis (EDA)** on healthcare patient data to extract meaningful insights related to:

- Treatment cost
- Recovery scores
- Hospital visits
- Readmission risk
- Department performance
- Patient behavior patterns

It uses Python data science tools to visualize and understand healthcare trends.

---

## 📦 Libraries Used

- Pandas → Data handling and analysis
- NumPy → Numerical operations
- Matplotlib → Basic plotting
- Seaborn → Advanced statistical visualization

---

## 📂 Dataset Handling

The dataset is loaded using Pandas, and a random sample is taken for efficient visualization.

### 📌 Why Sampling?
- Prevents overcrowded plots
- Improves visualization performance
- Helps in faster analysis

---

## 📊 Key Visualizations

### 🔹 1. Scatter Plot (Treatment Cost vs Recovery Score)
- Uses `hue=visit_type`
- Shows relationship between cost and recovery
- Helps identify patient patterns

---

### 🔹 2. Relational Plot (By Gender)
- Separate plots for male and female patients
- Shows variation across gender groups

---

### 🔹 3. Matplotlib vs Seaborn Comparison
- Side-by-side scatter plots
- Demonstrates difference between basic and advanced visualization tools

---

### 🔹 4. Distribution Analysis
- Histogram of treatment cost
- KDE plot for recovery score distribution
- ECDF plot for length of stay

---

### 🔹 5. Categorical Analysis
- Count plot of treatment types
- Bar plot of department vs treatment cost

---

### 🔹 6. Readmission Risk Analysis
- Stacked histogram by visit type
- Shows hospital readmission probability trends

---

### 🔹 7. Statistical Plots
- Box plot → Median, quartiles, outliers
- Violin plot → Distribution shape + density
- Strip plot → Individual data points
- Combined plot → All three in one view

---

### 🔹 8. Correlation Analysis
- Correlation matrix for numeric features:
  - Length of stay
  - Treatment cost
  - Recovery score
  - Readmission risk

---

### 🔹 9. Heatmaps
- Correlation heatmap (colored relationships)
- Masked heatmap (removes duplicate upper triangle)

---

## 📊 Key Insights

- Higher treatment cost does not always guarantee higher recovery score
- Readmission risk varies across visit types
- Department-wise differences exist in recovery patterns
- Strong correlations exist between key medical variables

---

## 🚀 Skills Learned

- Exploratory Data Analysis (EDA)
- Seaborn statistical visualization
- Matplotlib plotting
- Data sampling techniques
- Correlation analysis
- Heatmap interpretation
- Healthcare data insights extraction

---

## 📌 Purpose of Project

This project is designed to practice **real-world healthcare data analysis** and improve skills in:

- Data visualization
- Statistical understanding
- Python data science workflow
- Medical data interpretation
## ⭐ Author

**Fatima Ijaz**
