# 🛒 Amazon Product Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C72B0)
![Status](https://img.shields.io/badge/Status-Completed-success)

> A comprehensive exploratory data analysis (EDA) project on Amazon product listings — uncovering pricing patterns, discount strategies, and customer satisfaction trends.

---

## 📌 Project Overview

This project analyzes a real-world Amazon product dataset to extract meaningful business insights about pricing, discounts, ratings, and product performance across different categories.

**Dataset Source:** [Amazon Sales Dataset — Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)  
**Dataset Size:** 1,465 rows × 16 columns

---

## 🎯 Objectives

- Calculate key business KPIs (average prices, discount rates, ratings)
- Assess and improve data quality (missing values, duplicates, outliers)
- Visualize relationships between price, discount, and customer ratings
- Provide actionable insights for understanding market trends and customer behavior

---

## 🧰 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core programming language |
| Pandas | Data loading, cleaning & manipulation |
| Matplotlib | Plotting and visualization |
| Seaborn | Statistical visualizations |
| Jupyter Notebook | Interactive development environment |

---

## 📂 Project Structure

```
amazon-product-analysis/
│
├── amazon.csv               # Raw dataset
├── amazon_analysis.ipynb    # Main analysis notebook
└── README.md                # Project documentation
```

---

## 🔍 Analysis Workflow

### 1. Data Preparation
- Loaded and inspected the dataset (shape, dtypes, sample rows)
- Extracted `main_category` and `sub_category` from the combined category column
- Cleaned product names by removing special characters
- Converted price, discount, and rating columns to correct numeric types

### 2. Data Quality
- Handled **2 missing values** in `rating_count` using median imputation
- Confirmed **zero duplicate rows**
- Detected and analyzed outliers in price and rating distributions
- Performed sanity checks (e.g., discounted price > actual price)

### 3. Key KPIs

| KPI | Value |
| Total Products | 1,465 |
| Median Discounted Price | 799$ |
| Average Discount Rate | 4.0 |
| Median Actual Price | 1650$ |
| Average Rating | 4.1 |
| Max Discount | 94% |
| Min Discount | 0% |

### 4. Visualizations & Insights

- **Price Distribution** — Right-skewed; most products are budget-friendly (below ₹5,000)
- **Discount Strategy** — Most products discounted between 30%–60% (median ~50%)
- **Customer Ratings** — High satisfaction; median rating of 4.1 with few outliers below 3
- **Top Revenue Products** — Identified top 10 products by total revenue
- **Top Rated Products** — Products with high ratings but low sales flagged for review
- **Category Performance** — Top 3 categories ranked by total revenue
- **Price vs. Rating** — No strong linear correlation; high-priced products show more stable ratings

---

## 💡 Key Insights

- 📦 Amazon's catalog is dominated by **budget products** — 75% priced below ₹5,000
- 💸 A **consistent heavy-discount strategy** is in play, with most products discounted ~50%
- ⭐ **~95% of products** hold ratings of 4 stars or above — reflecting strong product quality
- 🔍 Some **highly rated products have low revenue** — indicating a marketing opportunity
- 📊 **Electronics dominate** the high-price segment with extreme outliers up to ₹80,000

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/amazon-product-analysis.git
cd amazon-product-analysis

# 2. Install dependencies
pip install pandas matplotlib seaborn jupyter

# 3. Launch the notebook
jupyter notebook amazon_analysis.ipynb
```

---

## 📧 Contact

Feel free to reach out for feedback or collaboration [[LinkedIn](https://www.linkedin.com/in/emansalahahmed/)](#)!

⭐ If you found this project useful, please consider giving it a star!
