# Sales-Insights
Sales Insights Data Analysis Project

## Project planning using AIMS grid –

**AIMS grid**: It is a project management tool which consists of four components to it.

1) **Purpose** (what to do exactly)

2) **Stack holders** (who will be involved)

3) **End result** (what do you want to achieve)

4) **Success criteria** (cost optimization and time save)

## Step 1 : ETL
Data cleaning was done using Excel.
Extract data using Power BI.
Transform the data using Power Query: Currency have been converted froom US$ to INR
                                      Filtered some of the rows which were repeating.
Load the data to build the dashboard.

## Step 2 : Building Dashboard

Dashboards/reports are created according to the requirement. What actually the company wants to look for and what is more important for the company is taken into consideration and then after the dashboard is created. There can be n number of variations to create a dashboard. Generally, the dashboard should look understandable and an ease to access.

**Formula** to create norm_amount column
= Table.AddColumn(#"Filtered Rows", "norm_amount", each if [currency] = "USD" or [currency] ="USD#(cr)" then [sales_amount]*75 else [sales_amount], type any)

Screenshots:

![Sales1](https://user-images.githubusercontent.com/70061236/173293915-6d31ed5e-13ee-4889-88f4-a3a36d5d8fcf.jpg)

![Sales2](https://user-images.githubusercontent.com/70061236/173293957-fb901a58-6206-4fb2-bfb0-33ba715ab6db.jpg)

![Sales3](https://user-images.githubusercontent.com/70061236/173293969-5b9febaa-f609-46b5-aeae-543528b53122.jpg)
