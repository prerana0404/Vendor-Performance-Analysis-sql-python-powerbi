# Vendor Performance Analysis -Retail Inventory & Sales


_End-to-end data analytics project to analyze vendor performance, inventory efficiency, procurement strategies, and profitability using SQL, Python, Statistical Analysis, and Power BI._

---

## Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools-and-technologies">Tools and Technologies</a>
- <a href="#project-structure">Project-Structure</a>
- <a href="#methods">Methods</a>
- <a href="#data-cleaning-preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#key-insights">Key Insights</a>
- <a href="#dashboard-output">Dashboard / Output</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>
- <a href="#author-contact">Author & Contact</a>
---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project analyzes large-scale supply chain data to identify top-performing vendors, procurement dependencies, inventory inefficiencies, and profitability trends. The analysis covers the complete analytics lifecycle, from data ingestion and database creation to statistical validation and dashboard reporting.

---
<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

Businesses often struggle with vendor dependency, slow-moving inventory, inefficient procurement decisions, and profitability optimization.

This project aims to:
- Identify top and low-performing vendors.
- Detect slow-moving inventory.
- Analyze procurement concentration risks.
- Evaluate the impact of bulk purchasing.
- Provide data-driven recommendations for improving profitability.

---
<h2><a class="anchor" id="dataset"></a>Dataset</h2>

### Source Files
- Sales.csv (25.65 Million Records)
- Purchases.csv (2.37 Million Records)
- Begin Inventory.csv (206K Records)
- End Inventory.csv (224K Records)
- Purchase Prices.csv (12K Records)
- Vendor Invoice.csv (5K Records)

### Total Records Processed
**28+ Million Records**

---
<h2><a class="anchor" id="tools-and-technologies"></a>Tools and Technologies</h2>

### Database
- SQL

### Programming
- Python
- Pandas
- NumPy

### Visualization
- Matplotlib
- Seaborn
- Power BI

### Statistical Analysis
- SciPy
- Hypothesis Testing
- Confidence Interval Analysis

---
<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>
```
vendor-performance-analysis/
├── notebooks/               #Jupyter Notebooks for EDA and Analysis
│   ├── Exploratory_Data_Analysis.ipynb
│   └── vendor_performance_analysis.ipynb 
|
├── scripts/                #Python scripts for ingestion and processing
│   ├── ingestion_db.py
│   ├── get_vendor_summary.py
│  
├── dashboards/            #Power BI Dashboard Files
│   └── vendor_performance_dashboard.pbix
|
├── vendor performance Report.pdf
└──.gitignore
└── README.md
```

<h2><a class="anchor" id="methods"></a>Methods</h2>

### Data Engineering
- Data Ingestion
- SQL Database Creation
- Data Validation
- Logging Implementation

### Data Processing
- SQL Joins
- Aggregations
- Feature Engineering

### Exploratory Data Analysis
- Summary Statistics
- Distribution Analysis
- Correlation Analysis
- Outlier Detection

### Statistical Analysis
- Confidence Interval Analysis
- Two-Sample T-Test

### Dashboard Reporting
- Power BI Dashboard Development

---
## Data Cleaning & Preparation
- Removed transaction with:
      - Gross Profit <= 0
      - Profit Margin <= 0
      - Sales Quantity = 0
- Created summary table with vendor-level metrics.
- Convert data types, handle outliers, merge lookup tables, and create new features for analysis.
---
<h2><a class="anchor" id="exploratory-data-analysis"></a>Exploratory Data Analysis (EDA)</h2>
 this section includes visualizations and statistical summaries to understand vendor performance, procurement patterns, inventory turnover, and profitability trends.
---

<h2><a class="anchor" id="key-insights"></a>Key Insights</h2>

### Vendor Contribution
- Top 10 vendors contribute approximately **65.4%** of total procurement.

### Bulk Purchasing
- Large orders receive significantly lower unit prices.
- Bulk purchasing reduces procurement costs by approximately **72%**.

### Inventory Analysis
- Multiple vendors recorded Stock Turnover below 1.
- Total Unsold Inventory Capital identified: **$216.19K**.

### Promotional Opportunities
- Identified **186 brands** with low sales but high profit margins.

### Profitability Analysis
- Top Vendors Mean Profit Margin: **65.08%**
- Low Vendors Mean Profit Margin: **61.69%**

### Statistical Validation
- T-Statistic: **7.8808**
- P-Value: **0.0000**
- Significant difference exists between top and low-performing vendors.

---
<h2><a class="anchor" id="dashboard-output"></a>Dashboard / Output</h2>

### KPI Metrics
- Total Sales
- Total Purchase
- Gross Profit
- Profit Margin
- Unsold Capital

### Visualizations
- Purchase Contribution Analysis
- Top Vendors by Sales
- Top Brands by Sales
- Low Inventory Turnover Vendors
- High Margin Low Sales Brands
![Power BI Dashboard](image/dashboard.png)
---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

### 1. Clone Repository
```bash
git clone https://github.com/prerana0404/Vendor-Performance-Analysis-sql-python-powerbi.git
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn scipy sqlalchemy
```

### 3. Create SQL Database
Import all CSV files into SQL tables.

### 4. Run Data Processing Scripts
```bash
python scripts/ingestion_db.py
python scripts/get_vendor_summary.py
```

### 5. Open and Run Notebooks
- 'notebooks/Exploratory_Data_Analysis.ipynb'
- 'notebooks/vendor_performance_analysis.ipynb'

### 6. Open Power BI Dashboard
- Open 'dashboards/vendor_performance_dashboard.pbix' in Power BI Desktop.

---

<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>
- Diversify vendor base to reduce risk
- Optimize bulk ordering strategies 
- Reprice slow-moving , high-margin inventory to improve sales
- clear unsold inventory strategically 
- improve marketing for underperforming vendors and brands

---
<h2><a class="anchor" id="results-conclusion"></a>Results & Conclusion</h2>

The project successfully identified vendor concentration risks, slow-moving inventory, procurement optimization opportunities, and profitability patterns.

The analysis demonstrated that:
- Vendor performance significantly impacts profitability.
- Bulk purchasing improves procurement efficiency.
- Inventory turnover plays a critical role in working capital management.
- Statistical testing confirmed meaningful differences between top and low-performing vendors.

---

<h2><a class="anchor" id="future-work"></a>Future Work</h2>

- Vendor Performance Forecasting
- Demand Forecasting Models
- Automated Inventory Replenishment
- Real-Time Power BI Integration
- Machine Learning Based Vendor Scoring

---
<h2><a class="anchor" id="author-contact"></a>Author & Contact</h2>

**Prerana Girame**
- Email:preranagirame2004@gmail.com
- LinkedIn: www.linkedin.com/in/prerana-girame