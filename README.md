# NYC Taxi Data Engineering Project

## What this project does
End-to-end data pipeline using PySpark on the NYC Yellow Taxi dataset.
Implements the Medallion Architecture (Bronze → Silver → Gold).

## Tech Stack
- PySpark
- Google Colab
- Parquet format
- NYC TLC Taxi Dataset (Jan 2023)

## Pipeline Layers
- **Bronze:** Raw Parquet data loaded with schema validation
- **Silver:** Cleaned data — nulls removed, new columns added (pickup_hour, trip_category)
- **Gold:** Aggregations — hourly revenue, trip category breakdown

## Key Results
- Processed 3M+ taxi trips
- Partitioned output by year/month/day for efficient querying
- Identified peak hours and trip patterns
