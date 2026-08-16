# Customer-Churn-Analysis
SQL + Python project analyzing customer churn patterns to uncover retention insight
About This Project

This is a personal data analytics portfolio project by Sahil Khan, a student with a growing interest in data and business insights. The goal of this project is to analyze customer churn behavior and uncover actionable business insights using SQL and Python.

Objective

To explore customer data, identify patterns behind why customers churn (leave), and translate those patterns into insights that could help a business improve customer retention.

Tools & Technologies
SQL (SQLite) – Data storage and querying
Python – Data analysis
pandas – Data manipulation
numpy – Numerical operations
matplotlib – Data visualization
seaborn – Statistical visualization
Jupyter Notebook – Development environment
Project Files
File	Description
CHURN_RETENTION_ANALYSIS.ipynb	Main Jupyter Notebook with all code, analysis, and visualizations
customer_churn_db.db	SQLite database containing the raw customer data
Project Report (PDF)	Summary report with findings and business insights
Project Workflow
Data Import – Connected to the SQLite database and loaded tables into pandas DataFrames
Data Cleaning – Handled missing values, corrected data types, removed inconsistencies
Exploratory Data Analysis (EDA) – Analyzed churn patterns across different customer segments
Visualization – Created charts using Matplotlib and Seaborn to highlight key trends
Insights & Recommendations – Summarized findings into a business-friendly report
Key Findings and Business Insights
Summary of Key Findings

The following findings emerge from the exploratory data analysis:

Overall churn rate is 28.6%. A significant share of customers have cancelled their subscriptions, above typical industry benchmarks, signaling a need for active retention measures.
Basic plan customers churn at roughly 4x the rate of Premium customers. A 60% churn rate on the Basic tier versus 14.3% on Premium is the most significant segment-level finding. It suggests Basic plan customers may be under-served, dissatisfied with value, or unable to commit long-term.
Escalations are a leading indicator of churn (correlation = 0.77). This is the strongest pairwise relationship in the dataset. Customers who escalate support complaints are substantially more likely to cancel. Since escalation events are observable in near real-time, this is a highly actionable early warning signal.
Premium customers contribute disproportionately to revenue. Total monthly charges for Premium subscribers ($218.93) are more than four times those of Basic subscribers ($52.95), reinforcing the business case for upselling and Premium retention.
Churn varies meaningfully by state. Geographic variation suggests market-specific factors — regional competition, service quality, economic conditions — contribute to churn differently across regions.
Average complaint volume is low (0.43 per customer), but the subset of customers who do complain — and especially those who escalate — show a dramatically elevated churn rate.
Business Recommendations

Based on the findings above, the following prioritized recommendations are offered:

Intervene immediately on escalated support tickets. With a 0.77 escalation–churn correlation, each escalated complaint should trigger an automated retention workflow — a personal outreach call, a service credit offer, or a plan upgrade offer. The cost of this intervention is almost certainly lower than the cost of churn and re-acquisition.
Redesign the Basic plan to reduce the perceived value gap. A 60% churn rate on the Basic tier is unsustainable. Consider enriching the Basic plan's feature set, adjusting pricing, or introducing a transitional "Starter Plus" tier. Alternatively, use CLTV data to identify high-value Basic customers for proactive upgrade offers.
Upsell Basic customers to Standard or Premium. Given that Standard (22.2%) and Premium (14.3%) customers churn far less, a structured upsell program targeting Basic subscribers — particularly those with high CLTV scores — could materially reduce overall churn while increasing revenue.
Launch targeted retention campaigns in high-churn states. Geographic churn variation warrants state-level segmentation of retention campaigns. High-churn states should receive additional customer success resources, localized offers, or regional support improvements.
Leverage CLTV for prioritized retention spend. The CLTV field in the subscription table provides a ready-made customer value ranking. Retention resources should be disproportionately allocated to high-CLTV customers who are showing churn risk signals, maximizing return on retention investment.
Monitor complaint count as an early churn signal. Even before escalation, multiple complaints from a single customer may predict churn. Setting a threshold (e.g., 2 or more complaints) to trigger proactive outreach could catch at-risk customers before they escalate.
How to Run This Project
Clone or download this repository
Make sure you have Python installed along with the required libraries:
   pip install pandas numpy matplotlib seaborn
Open CHURN_RETENTION_ANALYSIS.ipynb in Jupyter Notebook
Run the cells from top to bottom
About Me

Student | Aspiring Data Analyst

I'm passionate about turning raw data into meaningful business insights. This project is part of my growing data analytics portfolio as I build practical, hands-on experience with SQL, Python, and data visualization.

Feel free to connect or reach out with feedback!
