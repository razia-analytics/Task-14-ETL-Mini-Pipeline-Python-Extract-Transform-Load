# Retail Sales ETL

Simple ETL pipeline for a Kaggle retail sales CSV, built in **Google Colab**.

## Structure

* raw/        # original data
* processed/  # cleaned & enriched data
* output/     # final tables

## ETL Steps

1. **Extract**
   * Load Kaggle CSV into `raw/`

2. **Transform**

   * Remove missing values & duplicates
   * Standardize column names and datatypes
   * Create derived fields (margin, segment flags)

3. **Load**

   * Split into `customers`, `products`, `orders`
   * Export as CSV or load into SQLite

## Validation

* Row counts checked before & after
* Orders = processed rows
* Customer/product keys validated




