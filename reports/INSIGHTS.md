# Insights & Recommendations — Retail Analytics 2024

## 📌 Executive Summary
- **Total Revenue (2024):** ~€XX million  
- **Orders:** ~12k unique orders  
- **Average Order Value (AOV):** ~€YY  

Our analysis shows that promotions drive significant revenue uplift, but seasonality and channel mix also play an important role in overall performance.

---

## 🔎 Key Findings

### 1. Promotions
- Promo orders generated **~15% higher average revenue** compared to non-promo.  
- However, deep discounts risk lowering margins — best results came from moderate (5–20%) discounts.

### 2. Seasonality
- Revenue peaks in **July, November, and December**.  
- Holidays (e.g. Christmas, New Year) show strong demand spikes.  
- Weekends consistently outperform weekdays.

### 3. Categories & Channels
- **Top categories:** Electronics, Grocery, Clothing.  
- **Channel mix:** In-Store ~65%, Online ~35%. Online is steadily growing and shows stronger response to promotions.

### 4. Customers
- **Loyalty tiers:** Gold and Silver customers contribute a disproportionately high share of revenue.  
- Younger age groups (18–35) are more active online; older groups (46+) dominate in-store.

### 5. Model Performance
- A baseline **Linear Regression** model for predicting daily store revenue achieved:  
  - **R² ≈ 0.7**  
  - **MAE ≈ €4.5k**  
- Top positive drivers: promo share, holiday flag, online share.  
- Negative drivers: very high discount rates, cold weather days.

---

## ✅ Recommendations
1. **Run promotions strategically** — focus on months with natural demand spikes (Nov/Dec), and keep discounts moderate to protect margin.  
2. **Plan staffing & inventory** — boost coverage for weekends and peak months (Jul/Nov/Dec).  
3. **Grow online channel** — allocate more promo budget to online customers, where promo responsiveness is higher.  
4. **Loyalty programs** — invest in retaining Silver customers and converting them to Gold.  
5. **Pricing strategy** — track competitor prices closely in Electronics; consider selective price matching where sensitivity is high.  
6. **Next steps** — try tree-based ML models (RandomForest/XGBoost) for improved forecasting and add lag features for time-series revenue prediction.

---

📊 *This project demonstrates an end-to-end analytics pipeline: cleaning → EDA → feature engineering → machine learning → business recommendations.*
