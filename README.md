📑 DATA SCIENCE TASK 2: Exploratory Data Analysis and Sales Performance Analysis
🎯 Objective
The primary objective of this project was to perform an in-depth Exploratory Data Analysis (EDA) on a sales dataset to identify key trends, patterns, and anomalies, and to build a preliminary predictive model for sales performance.

💾 Dataset
Source: Global Superstore Sales Data (provided).

Key Columns Used: Sales, Profit, Discount, Region, Category, Product Name, Order Date.

🛠️ Project 1: General EDA Deliverables
This phase focused on data quality, statistical understanding, and foundational visualization.

1. Data Cleaning and Preprocessing 

Missing Values: No significant missing values were found in core columns.


Duplicates: 19 duplicates were identified and removed during the subsetting for Project 2, ensuring data integrity.


Outliers: Outliers in Sales and Profit were handled using the Interquartile Range (IQR) capping method to stabilize the distributions for statistical analysis and modeling.

2. Statistical Analysis 


Key Finding (Correlation): A strong negative correlation (−0.57) was found between Discount and Profit, indicating high discounts severely erode profit margins.

Distribution: Both Sales and Profit distributions are highly right-skewed, meaning a small number of high-value transactions account for a large portion of the revenue.

3. Visualizations 

P1_histogram_sales_profit.png: Displays the distribution of sales and profit.

P1_boxplot_sales_profit.png: Visualizes the spread and central tendency of the numerical variables.

P1_heatmap_correlation.png: Visually represents correlations between all numerical features.

📈 Project 2: Sales Performance Analysis Deliverables
This phase focused on time-based trends, variable relationships, and predictive modeling.

1. Key Visualizations 



Visualization	Key Finding
P2_time_series_sales.png	Shows clear yearly seasonality, with sales consistently peaking in the fourth quarter (Q4).
P2_scatter_profit_discount.png	Visually confirms that discounts above ≈20% frequently result in negative profit (losses).
P2_barplots_region_category.png	Identifies Central as the top-performing Region and Technology as the top-performing Category.

Export to Sheets

2. Predictive Model 

Model: Linear Regression Model.

Features Used: Profit and Discount.

Target: Sales.

Equation: Sales=94.15+(2.87×Profit)+(188.52×Discount)


Evaluation: The model's performance was weak, achieving an R 
2
  Score of 0.2708, indicating that Profit and Discount alone are insufficient to accurately predict Sales.

3. Insights and Actionable Recommendations 

Discount Optimization: Implement a strict discount ceiling (e.g., 20%) to stop profit erosion, only allowing higher discounts for strategic purposes (e.g., clearing old stock).

Resource Allocation: Prioritize marketing and inventory toward the high-performing Technology Category and the Central Region.

Capitalize on Seasonality: Align major campaigns and inventory stocking with the consistent Q4 peak demand observed in the time series plot.

Model Improvement: Future modeling efforts should include additional features, such as Shipping Cost and one-hot encoded categorical variables (Region, Category), to significantly improve predictive accuracy.

⚙️ Technical Requirements
Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn (for Linear Regression).

Code File: data_analysis_script.py (or your main Jupyter Notebook/Python file name).

Would you like to review any of these sections or elaborate on the code implementation details?
