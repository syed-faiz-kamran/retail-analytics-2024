Retail Analytics 2024 — End-to-End Data Analysis
📌 Business Problem

A mid-size retail chain wants to grow revenue and optimize promotions.
Management asked:

What drives sales?

Which promotions are effective vs. margin-killing?

Can we predict daily store revenue for staffing & inventory planning?

🛠️ Methods

Data Cleaning → fixed types, removed duplicates, handled missing & invalid values, standardized categories.

Exploratory Data Analysis (EDA) → KPIs (revenue, orders, AOV), sales drivers (category, channel, region), promotion effectiveness, and seasonality.

Feature Engineering → aggregated transactions into daily store-level dataset with discount, promo share, competitor gap, weather, and holiday flags.

Machine Learning → trained a baseline Linear Regression to predict daily store revenue.

📂 Files in Repo

data/

retail_sales_transactions_2024_clean.parquet → cleaned dataset (used in Colab)

retail_sales_transactions_2024_clean.csv → CSV version for GitHub preview

daily_store_revenue_features.parquet → engineered features

daily_store_revenue_features.csv → CSV version for preview

reports/

INSIGHTS.md → executive summary & recommendations

rev_by_category.csv, rev_by_channel.csv, monthly_revenue.csv → EDA summaries

notebooks/

01_cleaning.ipynb → data cleaning steps

02_eda.ipynb → exploratory analysis

03_features_ml.ipynb → feature engineering + ML

📊 Results (Highlights)

Promotions: increased average order revenue by ~15%

Seasonality: sales peaked in July, November, December

Channel mix: Online ≈ 35%, In-store ≈ 65% of revenue

Model: Baseline Linear Regression achieved R² ≈ 0.7, MAE ≈ €4.5k

✅ Recommendations

Run promotions strategically: positive uplift, but control discount depth to protect margin.

Staffing & inventory: boost for weekends + top months (Jul/Nov/Dec).

Grow online channel: allocate more promo budget where demand is rising.

Pricing: track competitor gap; selectively price-match in sensitive categories.

Next steps: try tree-based models (Random Forest, XGBoost), add lag features for time-series forecasting.

🖥️ Tech Stack

Python (Google Colab)

pandas, matplotlib, scikit-learn

Data size: 12k transactions (synthetic dataset for 2024)
