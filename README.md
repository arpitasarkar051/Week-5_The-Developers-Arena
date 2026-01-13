# Customer Sales Analysis 📊

This project analyzes customer purchasing patterns and overall sales performance using **Python** and **pandas**. The goal is to clean and combine sales and customer datasets, perform advanced data manipulation, and generate business insights with clear visualizations and a final report.[1][2][3]

## Project Objectives

- Analyze customer purchasing behavior and identify **top customers** by revenue and order frequency.[2][1]
- Evaluate product, regional, and monthly sales performance to uncover trends and seasonality.[4][1]
- Build a small analytics **dashboard** (4–5 visualizations) showcasing key business metrics.[5][2]
- Practice advanced pandas operations: grouping, aggregation, filtering, merging, datetime handling, and pivot tables.[3][6]

## Dataset Description

The project uses CSV files containing fictional customer and sales data (you can replace with your own real data):

- `sales_data.csv`  
  - Example columns: `order_id`, `order_date`, `customer_id`, `product`, `category`, `quantity`, `price`, `region`, `revenue`.[7][1]
- `customer_data.csv`  
  - Example columns: `customer_id`, `customer_name`, `segment`, `region`, `signup_date`.[7][4]
- `customer_churn.csv` (optional)  
  - Example columns: `customer_id`, `churned` (1 = churned, 0 = active) for simple retention analysis.[4]

Update column names in the notebook if your actual dataset differs.

## Project Structure

```text
.
├── customer_analysis.ipynb   # Main notebook with all analysis and visuals
├── sales_data.csv            # Sales dataset
├── customer_data.csv         # Customer dataset
├── customer_churn.csv        # Optional churn dataset
├── analysis_report.pdf       # Final business report
├── requirements.txt          # Python dependencies
└── README.md                 # Project overview and instructions
```

This layout follows common data analysis project patterns and keeps code, data, and documentation clearly separated.[8][3]

## Setup Instructions

1. **Clone or download** the repository  
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```

2. **Create and activate a virtual environment** (recommended)  
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```[3][9]

3. **Install dependencies**  
   Make sure `requirements.txt` includes packages like `pandas`, `numpy`, `matplotlib`, `seaborn`, and `jupyter`. Example:  
   ```bash
   pip install -r requirements.txt
   ```[2][9]

4. **Launch Jupyter Notebook**  
   ```bash
   jupyter notebook
   ```  
   Then open `customer_analysis.ipynb` from the browser interface.

## How to Run the Analysis

1. Open `customer_analysis.ipynb`.  
2. Run all cells from top to bottom:
   - **Data Loading & Exploration** – loads CSVs, checks structure, missing values.[1]
   - **Data Cleaning & Preparation** – handles missing values, converts dates, creates calculated columns like revenue and year-month.[5][1]
   - **Customer Analysis** – computes customer lifetime value, top customers, and regional distribution.[2][4]
   - **Sales Pattern Analysis** – monthly revenue, best-selling products, regional performance.[1][5]
   - **Advanced Analysis** – pivot tables, cross-selling pairs, basic retention/churn metrics.[6][4]
   - **Dashboard Creation** – generates 4–5 visualizations for KPIs and trends.[2][5]

3. Use the outputs and plots to write or update `analysis_report.pdf` with business-focused insights and recommendations.[10][11]

## Key Features & Techniques

- **Data Cleaning**
  - Handling missing values, removing invalid rows, fixing text inconsistencies (whitespace, case).[5][1]
- **Advanced Pandas**
  - `groupby`, multiple aggregations, complex filters with logical conditions, and string methods for text columns.[12][6]
  - Datetime conversion and extracting year, month, and day components.[6][1]
- **Merging & Joining**
  - Combining sales and customer datasets on `customer_id` and optionally joining churn information.[4][1]
- **Pivot Tables**
  - Revenue by region and month, revenue by category, and multi-metric pivots for more detailed summaries.[13][6]
- **Visualizations**
  - Line charts (monthly revenue), bar charts (top customers and regions), category performance, and heatmaps from pivot tables.[14][5]

## Testing & Validation

Basic checks you should perform:

- Confirm that data files load without errors and shapes are as expected.  
- Validate that `revenue = quantity * price` matches the source data where applicable.[1]
- Sanity check aggregations (e.g., total revenue equals sum of all row revenues, no duplicate order_id counts).[4][1]
- Manually inspect a few records to ensure joins and derived columns are correct.

You can also add simple assertion cells in the notebook to automatically verify these conditions.[3]

## Results & Business Insights

The final `analysis_report.pdf` summarizes:

- Total revenue, total customers, and average order value.  
- Top customers and top-performing products or categories.  
- Best-performing regions and observed seasonal trends in sales.  
- Simple retention or churn metrics and cross-selling opportunities (product pairs).[2][1][4]


[14](https://www.atmosera.com/blog/using-pandas-to-analyze-sales-data/)
[15](https://readme.md)
[16](https://github.com/najirh/Retail-Sales-Analysis-SQL-Project--P1)
[17](https://www.youtube.com/watch?v=5UhBnXWbCMY)
[18](https://inseaddataanalytics.github.io/INSEADAnalytics/ProjectsMenu.html)
[19](https://github.com/PetraLee2019/Python-Sales-Data-Analysis)
