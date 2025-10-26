📄 Global Superstore Sales Analysis
🎯 Project Goal

Conduct Exploratory Data Analysis (EDA) and Sales Performance Analysis on the Global Superstore dataset to identify key trends and build a preliminary predictive sales model.

💾 Dataset

File: global_superstore.csv

Key Columns: Sales, Profit, Discount, Region, Category, Date

📊 Key Findings
1. Profitability & Risk

Critical Correlation: Strong negative correlation (−0.57) between Discount and Profit. High discounts are the main cause of transactions resulting in losses.

Anomaly: High sales often correlate with high shipping costs → larger, higher-value orders are expensive to fulfill.

2. Performance & Trends

Seasonality: Sales show consistent yearly seasonality, peaking sharply in Q4.

Top Performers: Central Region and Technology Category have the highest total sales.

3. Predictive Model

Model: Linear Regression (Sales ~ Profit + Discount)

Evaluation: Weak performance (R² = 0.2708) → Profit and Discount alone are insufficient predictors of Sales.

✅ Actionable Recommendations

Optimize Discounting Strategy:
Implement a discount ceiling (~20%) to prevent negative profit margins. Apply higher discounts only for strategic inventory clearance.

⚙️ Tools & Libraries

Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
