# Amazon Sales — Exploratory Data Analysis

A comprehensive EDA project on 50,000+ Amazon sales records using Python. Uncovers regional revenue trends, seasonal demand patterns, product category performance, and customer satisfaction insights — with actionable business recommendations.

---

## Problem Statement

E-commerce businesses generate vast sales data but often lack clear visibility into what's driving revenue, which regions underperform, and when demand peaks. This project answers those questions through structured exploratory analysis and visualization.

---

## Dataset

- **Records:** 50,000+ Amazon sales transactions
- **Key columns:** `order_date`, `product_category`, `total_revenue`, `customer_region`, `payment_method`, `rating`

---

## Project Structure

```
amazon-sales-eda/
│
├── Amazon_1_.ipynb               # Main analysis notebook
├── amazon.csv                    # Raw dataset
├── README.md
└── images/
    ├── revenue_by_category.png
    ├── monthly_sales_trend.png
    ├── revenue_by_region.png
    ├── avg_rating_by_category.png
    └── payment_method_distribution.png
```

---

## Workflow

### 1. Data Loading & Inspection
- Loaded 50k+ records using `pd.read_csv`
- Checked null values, data types, shape, and descriptive statistics
- Assessed column completeness before analysis

### 2. Feature Engineering
- Parsed `order_date` into datetime format using `pd.to_datetime`
- Created `month_year` period feature using `dt.to_period('M')` for time-series aggregation
- Enabled month-over-month revenue trend tracking without external libraries

### 3. Exploratory Data Analysis

| Analysis | Chart Type | Business Question Answered |
|---|---|---|
| Payment method distribution | Bar chart | Which payment options do customers prefer most? |
| Revenue by product category | Bar chart | Which product lines generate the most revenue? |
| Monthly sales trend | Line chart | When do sales peak and when do they slump? |
| Revenue by region | Pie chart | Which geographic markets drive the most revenue? |
| Avg customer rating by category | Bar chart | Which categories have quality or satisfaction issues? |

### 4. Business Insights & Recommendations

**Payment Methods**
- Identified the dominant payment method used across transactions
- Recommended optimizing checkout pipeline for top payment method to prevent cart abandonment
- Suggested promotional campaigns (cashback) to shift volume toward lower-fee alternatives

**Product Categories**
- Identified top revenue-generating categories vs high-volume but low-revenue categories
- Recommended reallocating marketing budget toward highest-ROI categories
- Flagged underperforming categories for pricing and visibility review

**Seasonal Trends**
- Detected clear seasonal revenue spikes and off-peak slumps via monthly time-series
- Recommended scaling inventory and supply chain logistics ahead of peak months
- Proposed off-season promotional events to stimulate demand during slow periods

**Regional Performance**
- Mapped revenue distribution across customer regions using pie chart
- Identified dominant markets and untapped low-penetration regions
- Recommended localized advertising and shipping incentives for emerging regions

**Customer Satisfaction**
- Ranked product categories by average rating (out of 5.0)
- Flagged lowest-rated categories for quality assurance review
- Recommended bundling high-rated products with average-rated ones to boost overall perception

---

## Key Findings

- Sales exhibit **strong seasonality** with a distinct peak in specific months
- **One product category** drives a disproportionate share of total revenue
- **One region** accounts for the majority of sales, indicating concentration risk
- The **lowest-rated category** has significantly below-average customer satisfaction, signalling a quality gap

---

## Visualizations

Six chart types produced across the analysis:

| Chart | Library |
|---|---|
| Bar plots (category revenue, payment methods, ratings) | Seaborn |
| Line chart (monthly trend) | Matplotlib |
| Pie chart (regional revenue) | Matplotlib |
| Donut chart (top 5 loan purposes) | Matplotlib |
| Count plot (horizontal bar, loan purpose) | Seaborn |
| Grouped bar plots | Seaborn |

> All Seaborn charts updated to resolve `FutureWarning` deprecations by using the `hue` parameter correctly — production-quality, forward-compatible code.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| Pandas | Data manipulation & aggregation |
| NumPy | Numerical operations |
| Matplotlib | Base plotting |
| Seaborn | Statistical visualizations |
| Jupyter Notebook | Development environment |

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/Devinadh2403/amazon-sales-eda.git
cd amazon-sales-eda

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Launch the notebook
jupyter notebook Amazon_1_.ipynb
```

---

## Skills Demonstrated

- Data cleaning and null-value assessment
- Time-series feature engineering with Pandas datetime methods
- Multi-dimensional EDA across 5 business dimensions
- Business-oriented insight generation with actionable recommendations
- Production-quality, deprecation-free visualization code

---

## Author

**Kokkiligadda Devinadh**  
[LinkedIn](https://linkedin.com/in/devinadh-kokkiligadda) • kdevinadh01@gmail.com
