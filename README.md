# Census360 Sri Lanka

> An end-to-end data engineering and regional analytics project that transforms Sri Lankan census, population, housing, and administrative data into structured datasets, analytical indicators, ranked insights, predictive outputs, and interactive dashboards.

---

## Project Overview

Census360 Sri Lanka demonstrates a complete data workflow developed in Databricks.

The project processes raw demographic and housing datasets through Bronze, Silver, and Gold data layers. It cleans and combines regional records, creates analytical indicators, ranks geographical areas, validates outputs, and prepares dashboard-ready datasets for decision-making.

---

## Project Workflow

```text

                                        Raw Census and Housing Data
                                                    ↓
                                              Bronze Layer
                                                    ↓
                                               Silver Layer
                                                    ↓
                                               Gold Layer
                                                    ↓
                                        Feature Engineering and Scoring
                                                    ↓
                                        Regional Ranking and Prediction
                                                    ↓
                                        Interactive Dashboard Insights
                                        
```

### Bronze Layer

Stores the original source datasets with minimal transformation.

### Silver Layer

Cleans column names, standardizes data types, removes duplicate records, resolves regional identifiers, and combines population, housing, and administrative data.

### Gold Layer

Creates analytical features, opportunity scores, percentile-based tiers, regional rankings, summaries, predictions, and dashboard-ready tables.

---

## Key Project Features

- End-to-end Databricks data workflow
- Bronze, Silver, and Gold data architecture
- GN-division-level demographic analysis
- Population and housing data integration
- Administrative hierarchy standardization
- Data-quality validation and duplicate handling
- Demographic and household indicator creation
- Regional scoring and percentile-based tiering
- District, DS division, and GN division rankings
- Predictive model comparison and registration
- Interactive dashboard datasets
- GitHub-based version control and documentation

---

## Geographic Coverage

The final analytical dataset covers approximately:

| Administrative Level | Records |
|---|---:|
| Provinces | 9 |
| Districts | 25 |
| DS Divisions | 340 |
| GN Divisions | 14,008 |

---

## Repository Structure

```text
Census360-Sri-Lanka/
│
├── notebooks/
│   ├── 01_setup_and_file_verification
│   ├── 02_excel_and_csv_inspection
│   ├── 03_bronze_ingestion
│   ├── 04_silver_cleaning
│   ├── 05_gold_feature_engineering
│   ├── 06_ml_opportunity_score
│   └── 07_dashboard_queries
│
├── .gitignore
├── LICENSE
└── README.md
```

---

## Notebook Guide

| Notebook | Description |
|---|---|
| `01_setup_and_file_verification` | Configures the project environment and verifies the availability of source files |
| `02_excel_and_csv_inspection` | Inspects workbook sheets, headers, schemas, and raw data quality |
| `03_bronze_ingestion` | Loads the original datasets into Bronze Delta tables |
| `04_silver_cleaning` | Cleans, standardizes, deduplicates, and combines the regional datasets |
| `05_gold_feature_engineering` | Creates analytical indicators, scores, tiers, summaries, and rankings |
| `06_ml_opportunity_score` | Trains, compares, evaluates, logs, and registers predictive models |
| `07_dashboard_queries` | Creates SQL datasets used by the interactive dashboard |

---

## Main Analytical Outputs

The workflow produces:

- National summary indicators
- Province and district-level summaries
- DS division and GN division rankings
- Population and household indicators
- Demographic-share calculations
- Regional opportunity scores
- Percentile-based opportunity tiers
- Product and service priority views
- Predictive opportunity scores
- Model performance comparisons
- Strategic recommendation tables
- Dashboard-ready analytical datasets

---

## Data Architecture

```text
workspace.census360
│
├── bronze_*    Raw source tables
├── silver_*    Cleaned and standardized tables
└── gold_*      Analytical, ranked, predictive, and dashboard-ready tables
```

The architecture separates raw ingestion, data preparation, analytical processing, and presentation outputs to improve maintainability and reproducibility.

---

## Technology Stack

- Databricks
- Apache Spark
- PySpark
- Spark SQL
- Delta Lake
- MLflow
- Unity Catalog
- Pandas
- Git
- GitHub

---

## Dashboard

The Databricks dashboard provides interactive views for:

- National opportunity distribution
- District-level comparisons
- Regional priority rankings
- Product and service opportunity summaries
- High-priority GN divisions
- Regional drill-down analysis
- Predictive model insights
- Recommended actions

Dashboard filters support exploration by province, district, DS division, and opportunity tier.

---

## Data Availability

The original census, population, housing, and administrative source files are not included in this public repository.

The notebooks document the expected file structure, processing steps, transformations, validation logic, and analytical workflow without publishing credentials or private workspace information.

---

## Project Status

| Component | Status |
|---|---|
| Environment setup | Completed |
| Raw data inspection | Completed |
| Bronze ingestion | Completed |
| Silver cleaning | Completed |
| Gold feature engineering | Completed |
| Regional scoring and ranking | Completed |
| Predictive modelling | Completed |
| Model registration | Completed |
| Dashboard development | In progress |
| Final documentation | In progress |

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

Developed as a portfolio project demonstrating end-to-end data engineering, regional analytics, predictive modelling, dashboard development, model management, and version control using Databricks.