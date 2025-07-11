# Water-Supply-Business-Operations

# Water Supply Business Operations: End-to-End Data Analysis and Visualization

## Executive Summary
This repository showcases a complete data analysis pipeline for a small-scale water supply business. The project covers all aspects of data preparation, cleaning, analysis, visualization, forecasting, and reporting. Implemented in Python using pandas, seaborn, and matplotlib, this project demonstrates how data science methodologies can be applied to real-world operational data to generate actionable insights.

## Objective
The primary goal of this project was to analyze and optimize key aspects of the water delivery operations, including customer behavior, truck performance, and seasonal trends. The project supports strategic decision-making through data-driven insights.

## Dataset Description
The dataset used in this project is a simulated billing log for a water supply business, with the following fields:

- **Date**: Transaction date
- **Customer**: Customer name
- **Truck No**: Delivery vehicle identifier
- **Trip**: Number of trips made on a given day
- **Rate**: Billing rate per trip (INR)
- **Amount**: Total revenue per entry (Rate × Trip)
- **Challan No**: Unique invoice number

## Project Breakdown

### 1. Data Ingestion and Cleaning
- Loaded CSV data using `pandas`, ensured date parsing.
- Removed duplicate rows and entries with missing values.
- Applied logical constraints to filter invalid data (e.g., negative trips, rates outside range).
- Standardized data types for all numerical and categorical fields.

### 2. Feature Engineering
- Created new columns including:
  - Month (Period and Name)
  - Day of Week
  - Profit (Assuming fixed cost per trip)
  - Days Between Trips (per customer)

### 3. Exploratory Data Analysis (EDA)
- Revenue and Trip Trend Analysis:
  - Monthly revenue and trip count trends using line plots.
  - Weekly delivery distribution.

- Customer Insights:
  - Top 10 revenue-generating customers.
  - Declining customers based on recent activity.
  - Lifetime value segmentation (Regular, Medium, Rare).

- Operational Metrics:
  - Revenue and trips by truck.
  - Profitability comparison by truck.
  - Rate vs. Amount correlation using scatter plots.

- Seasonal Analysis:
  - Seasonal and weekday demand patterns.
  - Heatmap of revenue by weekday and month.

### 4. Forecasting
- Forecasted upcoming month's trips and revenue using historical mean.
- Computed monthly revenue growth rate to identify financial trends.

### 5. Business Rules & Validation
- Flagged duplicate Challan numbers for compliance check.
- Identified rates outside acceptable range (e.g., < ₹400 or > ₹1000).

### 6. Visualization Summary
- **Libraries Used**: `matplotlib`, `seaborn`
- **Plot Types**:
  - Line plots: Monthly revenue/trips
  - Bar plots: Top customers, seasonal demand, truck performance
  - Box plots: Trip and delivery frequency distributions
  - Scatter plots: Rate vs. amount
  - Heatmaps: Revenue by day and month

## Tools & Technologies
- Python 3.x
- Pandas, NumPy, Seaborn, Matplotlib
- Jupyter Notebook
- Git & GitHub (for version control and documentation)

## Directory Structure
```
water-supply-analysis/
│
├── main_analysis.ipynb     # Single notebook with complete analysis
└── README.md               # Project documentation
```

## Outcomes & Impact
- Enabled data-backed forecasting of trip demand and monthly revenue.
- Identified underperforming and high-value customers.
- Provided insights for optimizing truck scheduling and operational cost management.
- Supported strategic pricing by visualizing average monthly rates and profit margins.

## How to Run
1. Clone the repository:
```bash
git clone https://github.com/your-username/water-supply-analysis.git
cd water-supply-analysis
```

2. Open the Jupyter notebook:
```bash
jupyter notebook main_analysis.ipynb
```

3. Follow the notebook cells to run the full analysis.

## Author
**[Pranjal Patil]**  
_Data Scientist (Self-Employed)_

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Repository Link
Access the full project here: [GitHub Repository](https://github.com/your-username/water-supply-analysis)

---

