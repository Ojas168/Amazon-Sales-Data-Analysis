📊 Amazon Sales Data Analysis & Visualization
🔎 Project Overview

This project performs an end-to-end Data Analysis and Visualization workflow on an Amazon product sales dataset to uncover insights about pricing strategies, product popularity, customer satisfaction, and marketplace trends.

The goal was not just visualization, but transforming raw marketplace data into actionable business insights using industry-standard analytics practices.

🎯 Objectives

Clean and preprocess real-world e-commerce data

Perform Exploratory Data Analysis (EDA)

Build meaningful visualizations

Analyze correlations between pricing, discounts, and ratings

Extract business insights through data storytelling

Present findings in a portfolio-ready analytical format

🧠 Analytics Pipeline
1️⃣ Data Understanding

Inspected dataset structure using info() and describe()

Identified datatype inconsistencies and missing values

Validated column distributions before analysis

2️⃣ Data Cleaning & Preprocessing

Key transformations:

Removed currency symbols (₹) and commas from price columns

Converted object columns into numeric formats

Handled invalid values using coercion

Addressed missing data issues

df['actual_price'] = pd.to_numeric(
    df['actual_price'].astype(str)
    .str.replace('[₹,]', '', regex=True),
    errors='coerce'
)
3️⃣ Exploratory Data Analysis (EDA)

Performed structured diagnostics:

Null value analysis

Distribution inspection

Category frequency analysis

Statistical summaries

4️⃣ Data Visualization

Built visualizations using:

Matplotlib

Seaborn

Visuals included:

Category distribution bar charts

Price distribution histograms

Correlation heatmaps

Scatter plots (ratings vs discounts)

Log-scaled popularity analysis

5️⃣ Correlation Analysis
Relationship	Pearson r	Insight
Discount % vs Rating	-0.15	Discounts don’t influence satisfaction
Rating Count vs Rating	0.10	Popularity ≠ Quality
Actual vs Discounted Price	0.96	Pricing tiers preserved
📈 Key Insights
🛒 Marketplace Structure

Electronics dominate listings, indicating strong demand concentration in technology-related categories.

💰 Pricing Behavior

Price distribution is right-skewed, suggesting a marketplace focused on budget-to-mid-range consumers.

🏷️ Discount Strategy

Discounts do not significantly impact customer ratings, implying satisfaction depends on product experience rather than price reductions.

⭐ Popularity vs Quality

High review counts do not guarantee better ratings, highlighting the role of visibility and demand.

📊 Stable Pricing Hierarchy

Discounts are applied proportionally, maintaining relative product pricing positions.

🧩 Data Storytelling Conclusion

The Amazon marketplace reflects a demand-driven ecosystem where:

affordability drives volume,

discounts influence purchases but not satisfaction,

and popularity is shaped more by exposure than product quality alone.

🛠️ Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

📁 Project Structure
amazon-sales-analysis/
│
├── data/
│   └── amazon.csv
├── notebooks/
│   └── analysis.ipynb
├── visuals/
│   └── charts & plots
└── README.md
🚀 Skills Demonstrated

Data Cleaning & Wrangling

Exploratory Data Analysis

Statistical Interpretation

Data Visualization

Insight Extraction

Data Storytelling

Business Analytics Thinking

📌 Future Improvements

Interactive dashboard (Streamlit/Tableau)

Time-series sales analysis

Predictive rating modeling

Category-level profitability analysis

👤 Author

Ojas Vishwa Mohan
Aspiring Data Scientist | Python & Data Analytics Projects
