# 🔄 Data Preparation

The dataset consisted of **12 individual CSV files**, each representing one month of historical ride data.

An ETL (Extract, Transform, Load) process was implemented using **Microsoft Power Query** to consolidate all files into a single analytical dataset.

## ETL Workflow

### Extract

- Imported the twelve monthly CSV files.
- Validated schema consistency across datasets.

### Transform

Performed multiple transformation steps to prepare the data for analysis, including:

- Date formatting
- Data type conversion
- Duplicate detection
- Invalid record removal
- Creation of analytical variables

### Load

The cleaned dataset was loaded into Excel to support exploratory analysis, Pivot Tables, and dashboard creation.

---
