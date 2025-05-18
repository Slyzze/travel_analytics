# 🌍 travel_analytics

![DBT](https://img.shields.io/badge/dbt-v1.0+-green)
![Snowflake](https://img.shields.io/badge/Snowflake-Data%20Warehouse-blue)

A dbt + Snowflake analytics project analyzing international travel bookings.  
Inspired by  use cases, the project models booking, customer, and destination data to help analyze sales performance, revenue by region, and marketing channel effectiveness.

## 🚀 Project Highlights

- Transform raw booking data into clean analytical models
- Monthly revenue tracking per destination country
- Average price and booking volumes by continent
- Seed files for country-continent mapping and marketing channel classification
- Includes dbt tests for quality (not_null, unique)
- Uses Jinja with loops for dynamic SQL

## 🧱 Structure

```
models/
├── staging/
│   ├── stg_bookings.sql
│   ├── stg_customers.sql
│   └── stg_trips.sql
├── marts/
│   ├── mart_booking_summary.sql
│   └── mart_country_performance.sql
├── sources.yml
tests/
└── schema.yml
seeds/
├── countries.csv
└── marketing_channels.csv
```

## 📊 Example Use Cases

- Track top 5 travel destinations by language
- Compare revenue by continent
- Evaluate effectiveness of paid vs organic channels

## 🧪 Quality

Implemented dbt tests (`not_null`, `unique`) for core columns.  
Leverages dbt `ref()` and `source()` to ensure lineage and modularity.

## 🌐 Perfect for

- Education-focused analytics
- Travel industry data modeling
- Snowflake + dbt proof-of-concept

