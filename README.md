# Pharma Sales Analytics — Tableau

An exploratory business-intelligence project analyzing pharmaceutical sales across time, product classes, sales channels, geographies, distributors, and sales teams.

> **Data privacy note:** The packaged Tableau workbook includes an embedded Hyper extract. It contains transaction-level data and fields such as customer, distributor, and sales-representative names. Keep this repository **private** until you confirm that the dataset is authorized for public redistribution and contains no confidential or personal information.


## 📊 Dashboard Gallery

### 1. Executive Overview
![Executive Overview](docs/screenshots/Screenshot%202026-10-21%20020005.png)

### 2. Time Trend & Seasonality
![Time Trend](docs/screenshots/Screenshot%202026-10-21%20020023.png)

### 3. Product & Channel Analysis
![Product & Channel Analysis](docs/screenshots/Screenshot%202026-10-21%20020246.png)



## Project contents

- `Pharma_Sales_Analytics.twbx` — packaged Tableau workbook with its embedded extract.
- `docs/data_dictionary.md` — field definitions.
- `docs/analysis_notes.md` — selected findings and interpretation cautions.
- `docs/screenshots/` — place dashboard screenshots here after reviewing the workbook in Tableau.

## Analysis scope

The dataset contains **254,082 rows** and **18 fields**, covering 2017–2020. The workbook is organized into worksheets, dashboards, and a story for exploring executive KPIs, trends, products, channels, markets, sales teams, and data-quality/concentration questions.

## Selected findings

These figures were calculated from the supplied CSV and are descriptive, not causal:

- Net sales total approximately **11.80 billion** in the dataset's numeric sales units; no currency is specified in the source.
- Germany contributes approximately **94.2%** of net sales.
- Pharmacy contributes approximately **52.7%** of net sales; Hospital contributes approximately **47.3%**.
- The Analgesics product class is the largest class by net sales at approximately **2.37 billion**.
- **2,633 rows (about 1.04%)** have negative sales values. These may represent returns, corrections, or data issues; the source does not identify the reason.
- The top 10 distributors account for approximately **92.6%** of net sales, indicating high distributor concentration that merits validation.
- 2018 has the highest total sales, but also a much larger number of rows than other years. Compare row counts and average sales per row before interpreting this as underlying business growth.

See [`docs/analysis_notes.md`](docs/analysis_notes.md) for caveats.

## Open the workbook

1. Install/open Tableau Public Desktop.
2. Select **File → Open** and choose `Pharma_Sales_Analytics.twbx`.
3. Review the workbook and confirm filters, dashboards, and story behavior in Tableau before publishing.
4. If you publish the workbook to Tableau Public, add the public visualization URL here.

## Tools

- Tableau Public Desktop
- Tableau Packaged Workbook (`.twbx`) with Hyper extract
- CSV-based exploratory analysis for the descriptive findings above

## Reproducibility and limitations

The original CSV is not duplicated in this repository because the workbook already includes an extract. Source data currency, data licensing, and the business meaning of negative sales are not specified in the supplied file. The workbook has been structurally inspected, but visual behavior should be verified in Tableau Desktop before publishing.
