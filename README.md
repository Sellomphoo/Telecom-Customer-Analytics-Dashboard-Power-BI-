# Telecom Customer Analytics Dashboard (Power BI)

## Overview

An interactive Power BI dashboard that analyses a telecom company's customer base of **7,043 customers**. It shows who the customers are, how they pay, which contracts and internet services bring in the most revenue, and where they are located, so a business can see its customer base and revenue drivers at a glance.

**Dashboard title:** Telecom Customer Analytics
**Tagline:** Better Insights | Smarter Decisions

## Objectives

1. Summarise the customer base: size, revenue, average monthly charge, households and referrals.
2. Understand customer demographics by age group, gender and marital status.
3. Identify which contract types and internet services drive revenue.
4. Show how customers pay and where they are located.
5. Let users filter the whole dashboard by **Gender** and **Customer Status**.

## Dataset

- **Records:** 7,043 customers, each with one row of data
- **Fields used:** Customer ID, Gender, Age Group, Married, Number of Dependents, Number of Referrals, Contract, Internet Type, Payment Method, Monthly Charge, Total Charges, Total Revenue, Customer Status, City, Latitude, Longitude
- **Source:** [add dataset link here]

## Dashboard contents

**KPI cards**
- Number of Customers: **7,043** (distinct count of Customer ID)
- Total Revenue: **21.37M**
- Average Monthly Charge: **63.60**
- Number of Dependents: **3,301**
- Number of Referrals: **13,747**

**Visuals**
- **Total Customers by Age Group:** column chart
- **Total Revenue by Contract:** column chart
- **Married Status:** donut chart
- **Payment Method:** donut chart
- **Total Charges by Internet Type:** bar chart
- **Customer Locations:** filled map by city, using latitude and longitude

**Slicers:** Gender and Customer Status

## Key insights

- **Customer base:** 7,043 customers generate 21.37M in total revenue, about 3,030 per customer, with an average monthly charge of 63.60.
- **Age:** customers aged 25-64 make up about 73% of the base, with a balanced spread across those four bands (1,248 to 1,317 customers each). Ages 18-24 are the smallest group (779, about 11%).
- **Contracts:** two-year contracts generate the most revenue (9.0M, about 42%). One-year and month-to-month contracts contribute equally (6.2M each, about 29%).
- **Internet type:** Fiber Optic is the main driver at 9.8M, about two-thirds of internet charges. DSL (3.5M) and Cable (1.7M) trail well behind.
- **Payment:** most customers pay by bank withdrawal (55.5%), followed by credit card (39.0%). Mailed cheque is rare (5.5%).
- **Households:** the base is split almost evenly between married (48.3%) and unmarried (51.7%) customers.
- **Geography:** customers are concentrated in California's major metro areas, especially around Los Angeles and the Bay Area.
- **Referrals:** the base averages about 2 referrals per customer (13,747 in total), which suggests word of mouth is working.

## Design decisions and limitations

- **Customer analysis, not churn analysis.** The dataset contains a Customer Status field, but this dashboard is deliberately scoped to understanding the customer base and revenue. It does not report churn rates, so it makes no claims about why customers leave.
- **Revenue vs customer count.** The contract chart shows total revenue, not customer counts. It shows which contracts generate the most revenue, not which have the most customers or the highest spend per customer.
- **Different revenue measures.** Total Revenue (21.37M) and Total Charges by Internet Type (about 15.0M across the three types) are different measures, so they are not expected to match.
- **Single-table model.** All fields come from one table, which is enough for this scope. A larger project would split it into fact and dimension tables.
- Findings describe this dataset only and should not be generalised to other telecom companies.

## Tools used

- Power BI Desktop: KPI cards, column, bar and donut charts, filled map, slicers, DAX measures
- Data cleaning and preparation before visualisation

## How to use

1. Download `Telecom.pbix`.
2. Open it in **Power BI Desktop**.
3. Use the Gender and Customer Status slicers to filter every visual on the page.

## Author

**Sello Mpho** · Bloemfontein, South Africa
[Portfolio](https://mpho-sello.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/mpho-sello-692193241) · sellompho1601@gmail.com
