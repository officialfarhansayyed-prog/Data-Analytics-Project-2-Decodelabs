# E-Commerce Exploratory Data Analysis (EDA)

## 📌 Overview
This project delivers a comprehensive Exploratory Data Analysis (EDA) on an e-commerce dataset containing 1,200 transactional records across 14 metrics[cite: 1]. The primary goal is to identify underlying revenue patterns, customer purchasing behaviors, promotional impacts, and operational optimizations using Python[cite: 1].

---

## 🛠️ Tools, Libraries & Environment
* **Environment:** Google Colab[cite: 1]
* **Language:** Python 3.x[cite: 1]
* **Data Manipulation:** `pandas`, `numpy`[cite: 1]
* **Data Visualization:** `matplotlib`, `seaborn`[cite: 1]
* **Version Control & Documentation:** GitHub & Markdown[cite: 1]

---

## ⚙️ Steps Executed

### 1. Data Forensics & Cleaning
* **Missing Value Imputation:** Detected 309 missing values in `CouponCode` (~25.75% missingness)[cite: 1]. Replaced missing entries with `"NO_COUPON"` to preserve analytical integrity without dropping valid rows[cite: 1].
* **Integrity Checks:** Verified dataset dimensions (1,200 rows × 14 columns) and confirmed zero duplicate records[cite: 1].

### 2. Descriptive & Statistical Analysis
* **Five-Number Summary:** Calculated standard statistical metrics (Mean, Median, Standard Deviation, Min, Max, Quantiles) for numerical features (`Quantity`, `UnitPrice`, `ItemsInCart`, `TotalPrice`)[cite: 1].
* **Distribution Check:** Identified a right-skewed revenue distribution, where the mean order value ($1,053.97) exceeds the median ($823.62)[cite: 1].

### 3. Outlier Diagnostics
* Applied the **Interquartile Range (IQR)** rule ($Q3 + 1.5 \times IQR$) to detect extreme order values[cite: 1].
* Located **8 upper-tail outlier orders** exceeding the upper bound threshold of $3,330.41[cite: 1].

### 4. Bivariate Analysis & Pivot Summaries
* **Correlation Analysis:** Evaluated relationships using a Pearson Correlation Heatmap, discovering strong positive ties between `TotalPrice` and both `UnitPrice` (0.65) and `Quantity` (0.62)[cite: 1].
* **Product Ranking:** Plotted gross revenue across product lines, identifying **Chairs ($195,620)** and **Printers ($195,612)** as top drivers, while **Phones ($151,722)** yielded the lowest sales[cite: 1].
* **Pivot Table Aggregation:** Built multi-variable pivot tables comparing gross revenue across product categories and customer payment methods[cite: 1].

---

## 📊 Key Business Insights
1. **Bulk & High-Ticket Drivers:** Total transaction revenue is heavily driven by item quantity and individual unit cost rather than cart item volume[cite: 1].
2. **Category Performance:** Office furniture and printing hardware yield the highest sales returns across all channels[cite: 1].
3. **Promotional Adoption:** Approximately 74.25% of orders utilized promotional coupons (`FREESHIP`, `SAVE10`, `WINTER15`)[cite: 1].

---

## 💡 Strategic Recommendations
* **Bundle High-Ticket Hardware:** Offer targeted package deals for high-value hardware (e.g., Printers and Laptops) to maximize total cart revenue[cite: 1].
* **Optimize Discount Strategies:** Evaluate profit margins on coupon-bearing orders against the 25.75% non-coupon orders to refine discount thresholds[cite: 1].
