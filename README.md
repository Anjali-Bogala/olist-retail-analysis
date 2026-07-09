# Olist Retail Sales Intelligence Platform

## Project Overview
End-to-end data analysis project on the Brazilian Olist 
e-commerce dataset (100k+ orders, 9 tables). Built to simulate 
a real industry analytics engagement — from raw messy data to 
executive-ready insights and a Power BI dashboard.

## Status
In Progress 

## Tech Stack
Python · pandas · SQL (SQLite) · Power BI · Git

## Dataset
Brazilian E-Commerce Public Dataset by Olist (Kaggle)
99,441 orders · 9 related tables · 2016–2018

## Key Findings So Far
- 93.4% of orders arrive before estimated delivery date
- Late delivery drops customer satisfaction from 4.2★ to 2.26★
- Late orders paradoxically have the highest avg order value (₹134)
- SP volume dilution effect confirmed across 25 states
- Watches/gifts is a hidden high-efficiency revenue category

## Notebooks
01_data_understanding | Load all 9 tables, .info() audit, data quality findings.
02_schema_mapping | ERD, primary key verification, join validation.
03_data_cleaning | Cleaning pipeline, date fixes, NULL handling, master table. 
04_sql_setup | SQLite queries, business intelligence, delivery analysis.

## Structure
data/cleaned/    → analysis-ready cleaned CSVs
notebooks/       → Jupyter notebooks (one per project phase)
reports/         → charts and executive summary 
