# sales-data-quality-dashboard
# Sales Data Quality Dashboard

An automated sales data validation, cleaning, and reporting tool built with **Google Sheets and Google Apps Script**.

This project demonstrates how scripting and spreadsheet tools can be used to improve data quality, automate repetitive processes, and turn raw sales data into actionable business insights.

## Project Overview

The Sales Data Quality Dashboard processes raw sales records through an automated workflow that identifies data quality issues, prepares clean datasets, calculates key business metrics, and generates an interactive dashboard.

The project uses fictional sample sales data and is designed to demonstrate practical data analysis, data validation, automation, and reporting techniques.

## Key Features

- **Automated Data Quality Checks:** Identifies missing required fields, duplicate records, invalid values, and inconsistent data.
- **Data Cleaning:** Excludes records with critical errors and standardizes minor inconsistencies.
- **Sales Metrics:** Calculates order counts, revenue, and average order value, with separate reporting for completed, pending, and cancelled orders.
- **Product and Regional Analysis:** Breaks down sales performance by product and region.
- **Data Quality Reporting:** Summarizes records received, retained, excluded, QA findings, and retention rate.
- **Interactive Dashboard:** Displays key performance indicators, revenue breakdowns, order status, and data quality summaries.
- **One-Click Refresh:** A dashboard button runs the complete workflow, updating the underlying analysis and visualizations.

## Tools & Technologies

- Google Sheets
- Google Apps Script
- JavaScript
- Google Sheets Charts

## Workflow

The project uses a sequential workflow:

1. **Validate:** Run data quality checks against the raw sales data.
2. **Clean:** Use QA results to exclude invalid records and standardize minor inconsistencies.
3. **Analyze:** Calculate summary metrics and product and regional breakdowns using the cleaned dataset.
4. **Report:** Update dashboard metrics, data quality summaries, and visualizations.

## Business Rules

- Order IDs must be unique. Exact duplicate records are flagged, while conflicting records sharing an Order ID are treated as errors.
- Required fields must be populated.
- Invalid dates, regions, quantities, prices, and statuses are flagged.
- Minor inconsistencies, such as differences in status capitalization, are standardized where appropriate.
- Records with critical errors are excluded from the cleaned dataset.
- Completed, pending, and cancelled orders are tracked separately.
- Completed revenue and pending revenue are reported separately. Cancelled order value is tracked independently and excluded from completed revenue.

## Project Structure

| File | Description |
|---|---|
| `Code.gs` | Contains the Apps Script functions for data validation, cleaning, analysis, and dashboard generation. |
| `README.md` | Project overview, features, workflow, and business rules. |

## Running the Project

The script is designed to run within its associated Google Sheets workbook.

1. Open the Google Sheets workbook.
2. Navigate to the Dashboard tab.
3. Click **Refresh Dashboard** to run the complete workflow.
4. Review the updated metrics, charts, and data quality summary.

The script requires access to the associated workbook and appropriate authorization to run.

## Project Goals

This project was developed to demonstrate practical skills in:

- Data validation and quality assurance
- Data cleaning and transformation
- JavaScript and Google Apps Script
- Spreadsheet automation
- SQL-inspired data analysis concepts
- Metric development and business reporting
- Dashboard design and data visualization
