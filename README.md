# Supply-Chain-Analysis-Project-Using-Python-
analyze a real-world supply chain dataset using Python, Pandas, Matplotlib, Seaborn, Scikit-Learn build a machine learning model

📦 End-to-End Supply Chain Analysis & Late Delivery Prediction
An enterprise-grade data analytics and machine learning project analyzing 170,000+ global e-commerce orders to uncover delivery bottlenecks, quantify financial losses, and predict shipment delay risks proactively.

🚀 Project Overview
In modern e-commerce, supply chain transparency and on-time fulfillment directly govern customer trust and retention. This project investigates an extensive supply chain dataset spanning from 2015 to 2018. By combining rigorous Exploratory Data Analysis (EDA), bottleneck detection, temporal trend analysis, and a predictive Machine Learning pipeline, this project shifts fulfillment strategy from reactive firefighting to proactive risk mitigation.

📊 Key Performance Indicators (KPIs) & Findings
Total Orders Analyzed: 172,765 orders across multiple global markets and shipping modes.

Late Delivery Rate: 60.09% of total orders experienced delivery delays, highlighting severe systemic bottlenecks.

Profitability Impact: While total accumulated profit reached $7.5M, delayed shipments caused a significant profit bleed and loss exposure of $2.2M.

Delay Magnitude: The 90th percentile delay is capped at 3 days, indicating process-driven friction rather than isolated logistical anomalies.

🛠️ Tech Stack & Libraries
Language: Python 3.x

Data Manipulation & Analysis: Pandas, NumPy

Data Visualization: Matplotlib, Seaborn

Machine Learning & Imbalance Handling: Scikit-Learn (RandomForestClassifier), Imbalanced-Learn (SMOTE)

⚙️ Project Workflow & Architecture
1. Data Cleaning & Preprocessing
Removed redundant columns, fully missing attributes (Product Description, Order Zipcode), and administrative entries like canceled shipments.

Converted date-time fields to structured timestamps to engineer temporal features (order_month, order_day, order_hour, Delay_Days, Is_Delayed).

2. Bottleneck Detection & Root Cause Analysis
Regional & Market Vulnerabilities: Discovered chronic delay concentrations in complex routing regions such as Southeast Asia and Central Africa.

Shipping Mode Analysis: Identified Standard Class shipping as the primary contributor to high-volume order processing delays compared to expedited methods (First Class, Same Day).

Temporal Insights: Analyzed monthly and hourly transaction trends to pinpoint peak operational strain periods.

3. Machine Learning Predictive Modeling
To solve the business problem of unpredictable delivery timelines, a classification model was built to predict delays before dispatch:

Feature Engineering: Utilized features including scheduled shipping days, sales per customer, total sales, profit per order, product price, order month, and order hour.

Handling Class Imbalance: Applied SMOTE (Synthetic Minority Over-sampling Technique) on training data to balance delayed vs. on-time classes.

Model Evaluation (RandomForestClassifier):

Accuracy: 69.66% (~70%)

Precision: 79.62% (High reliability when flagging high-risk late orders)

Recall: 66.55%

📈 Key Visualizations Included in Notebook
Profitability & Delay Distributions: Dual-panel charts mapping order count percentages and profit leakage across delay days.

Multi-Category Bottleneck Grids: 2x3 subplot grids breaking down delay percentages across regions, market segments, and shipping modes.

Root Cause Driver Analysis: Horizontal ranking of primary factors contributing to late deliveries in high-risk zones.

Time Series Trends: Multi-axis seasonality trends across months, days of the week, and hours of the day.

💼 Business Recommendations & Strategic Impact
Proactive Risk Flagging: Integrate the trained Random Forest classifier into the order dispatch pipeline to automatically flag high-risk delayed shipments in real time.

Logistics SLA Optimization: Renegotiate Service Level Agreements (SLAs) with regional carriers operating in chronically delayed corridors (e.g., Southeast Asia).

Inventory Relocation: Position high-demand product lines closer to high-volume customer clusters to minimize transit turnaround times.

⚙️ How to Run the Code Locally
Clone the repository:

Bash
git clone https://github.com/your-username/supply-chain-analysis.git
Install dependencies:

Bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
Open the Jupyter Notebook and run cells sequentially:

Bash
jupyter notebook "Supply Chain Analysis Project Using Python.ipynb"
Created with ❤️ by Ankit Joshi
