# Mobile Money Data Pipeline and Fraud Analytics

This project looks at how mobile money transaction data can be collected, stored, cleaned and prepared for analysis.

The dataset used is PaySim, a synthetic mobile money dataset based on transaction patterns from a real mobile money service.

The goal is to build a simple end-to-end data pipeline and then use the cleaned data to study transaction activity and fraud patterns.

## Project plan

The pipeline will use:

- Python for data ingestion
- PostgreSQL for storage
- dbt for data cleaning and transformation
- SQL for analysis
- Power BI for reporting

## Pipeline

```text
PaySim CSV
    ↓
Python
    ↓
PostgreSQL
    ↓
dbt
    ↓
Analytics tables
    ↓
Power BI
```

## Questions I want to answer

- Which transaction types are used the most?
- How much money moves through each transaction type?
- When is transaction activity highest?
- Which transaction types contain fraudulent activity?
- How do fraudulent transactions differ from normal transactions?
- Are there unusual balance patterns around fraudulent transactions?
- Which accounts appear repeatedly in suspicious transactions?

## Project structure

```text
data/           local raw data files
ingestion/      Python scripts for loading data
sql/            SQL used during analysis
dbt/            dbt models and transformations
dashboards/     Power BI files and screenshots
docs/           notes, diagrams and project documentation
```

## Dataset

PaySim will be kept outside GitHub because the raw dataset is large.

The source will be documented here once the data is added locally.
