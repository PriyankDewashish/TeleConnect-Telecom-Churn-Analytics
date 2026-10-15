# TeleConnect - Telecom Customer Churn Analytics

A Power BI portfolio project exploring customer churn, retention, plan
performance, and regional customer distribution for a fictional Indian
telecom provider.

> **Data notice:** This project uses a synthetic dataset created for
> learning and portfolio demonstration. It is not actual customer data
> from Airtel, Jio, or any other telecom company.

## Dashboard Preview

<img width="497" height="281" alt="image" src="https://github.com/user-attachments/assets/879ac4b7-a270-4f3f-a0ee-0f9ce4ff40de" />

A PDF export of the dashboard is also available in the `screenshots/`
folder.

## Business Objective

This project answers practical business questions: - How many customers
does the provider have? - How many customers have churned, and what are
the churn and retention rates? - How does customer distribution differ
across monthly, quarterly, and yearly plans? - Which regions have the
largest customer bases? - Which plan types have higher churn rates? -
What reasons are most frequently associated with churn?

## Key Results

Based on the generated dataset of 1,000 customers:

  KPI                    Result
  -------------------- --------
  Total customers         1,000
  Churned customers         157
  Retained customers        843
  Churn rate              15.7%
  Retention rate          84.3%

Churn rate is churned customers divided by total customers. Retention
rate is retained customers divided by total customers. Both use the same
customer population and should add up to 100%.

## Dashboard Visuals

1.  **Customer Distribution by Plan Type** --- compares monthly,
    quarterly, and yearly plan customer counts.
2.  **Customer Distribution by Region** --- compares customer counts
    across regions.
3.  **Churn Rate by Plan Type** --- compares churn percentages rather
    than raw churn counts.
4.  **Top Churn Reasons** --- shows recorded reasons for churn,
    excluding `Not Applicable`.
5.  **Churned Customers by Plan Type** --- compares churned customer
    counts by plan duration.

The report also includes KPI cards for total customers, churned
customers, churn rate, and retention rate, plus slicers for region, plan
type, and churn status.

## Tools Used

-   **Microsoft Power BI Desktop** --- report building and visualization
-   **Power Query** --- data import and preparation
-   **DAX** --- KPI calculations
-   **CSV** --- dataset format

## Dataset

The `data/` folder contains: - `telecom_customer_churn.csv` --- 1,000
synthetic customer records - `teleconnect_data_dictionary.csv` ---
column descriptions

Each row represents one customer. Fields include customer ID, state,
region, plan name and type, plan price, monthly-equivalent price, daily
data allowance, tenure, payment method, reported network issues, support
calls, churn status, and churn reason.

The dataset was generated with unique customer IDs and no missing
values. Because it is synthetic, patterns are illustrative and should
not be treated as evidence about a real telecom market.

## Repository Structure

``` text
TeleConnect-Telecom-Churn-Analytics/
├── README.md
├── data/
│   ├── telecom_customer_churn.csv
│   └── teleconnect_data_dictionary.csv
├── dashboard/
│   └── TeleConnect_Churn_Dashboard.pbix
└── screenshots/
    ├── dashboard_overview.png
    └── TeleConnect_Dashboard_Report.pdf
```

If you have not added the `.pbix` file yet, save the report from Power
BI Desktop and upload it to `dashboard/`. If your screenshot or PDF uses
a different filename or folder, update the preview path above to match
your repository.

## Limitations

-   The company and customer records are fictional.
-   The dataset is a customer-level snapshot, not a monthly historical
    dataset.
-   The analysis compares customer groups; it does not prove that any
    factor causes churn.
-   This project is for learning and portfolio demonstration, not
    operational business decisions.

## Future Improvements

-   Add a plan-level summary with customer counts and churn rates.
-   Add a retention-priority view for customer segments with
    comparatively high churn.
-   Add time-based snapshots to analyze churn trends over time.
-   Improve accessibility with larger labels, clear contrast, and
    consistent spacing.

## Author

**Priyank Dewashish**\
Data Analytics Portfolio Project
