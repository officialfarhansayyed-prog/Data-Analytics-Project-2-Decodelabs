# Exploratory Data Analysis (EDA) - E-Commerce Dataset

## 📌 Project Overview
This project performs an end-to-end Exploratory Data Analysis on an e-commerce dataset containing 1,200 transaction records across 14 metrics.


## 📊 Key Insights & Findings
- **Revenue Drivers:** Chairs ($195,620) and Printers ($195,612) generated the highest overall revenue.
- **Correlation Metrics:** Total order price shows strong positive correlation with Quantity (0.62) and Unit Price (0.65).
- **Data Cleaning:** Imputed 309 missing values in `CouponCode` with `"NO_COUPON"` to maintain data integrity.
- **Outlier Diagnostics:** Identified 8 upper-tail outlier orders exceeding $3,330.41 using the Interquartile Range (IQR) method.

## 💡 Business Recommendations
1. Promote high-ticket product bundling to leverage strong volume and unit price correlations.
2. Track coupon vs non-coupon conversion performance to optimize promotional discount strategies.
