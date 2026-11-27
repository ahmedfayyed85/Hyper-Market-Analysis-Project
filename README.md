Hyper Market Sales Analysis

An interactive Power BI project for exploring hypermarket sales, profitability, customer activity, products, stores, and returns. The report is built from a Power BI Project (`.pbip`) with a separate semantic model and report definition.

## Project Contents

- `Hyper-market-data.pbip` — Power BI Project entry point.
- `Hyper-market-data.Report/` — report pages, visuals, and report resources.
- `Hyper-market-data.SemanticModel/` — model tables, relationships, Power Query expressions, and DAX measures.
- `Hyper-Data/` — source CSV files used by the project:
  - `Sales 2017.csv` and `Sales 2018.csv`
  - `Calendar.csv`
  - `Customers.csv`
  - `Products.csv`
  - `Region.csv`
  - `Returns.csv`
  - `Stores.csv`
- `images/` — project screenshots.

## Analysis Highlights

The semantic model includes measures for:

- Total sales, cost, gross profit, and gross margin.
- Quantity sold, customers, products, and average sales per customer.
- Returns and return rate.
- Month-over-month changes for key metrics and sales growth.

The report can be filtered and explored using the dimensions in the model, such as calendar date, product, customer, region, and store.

## Requirements

- Microsoft Power BI Desktop with support for Power BI Project (`.pbip`) files.
- The CSV source files in the `Hyper-Data` folder.

## Open the Project

1. Clone or download this repository.
2. Open `Hyper-market-data.pbip` in Power BI Desktop.
3. If Power BI asks you to configure data sources, update the Power Query source paths to point to the `Hyper-Data` folder in your local copy.
4. Refresh the data, then open the report pages to explore the analysis.

## Data Source Configuration

The semantic model currently contains Power Query expressions that refer to a local folder path from the original author's computer. Those paths will not exist on another machine. Before refreshing, update the folder references in Power BI Desktop so they point to the repository's `Hyper-Data` directory. The CSV files are included in this repository.

## Git Notes

The `.gitignore` excludes Power BI local settings and cache files under `.pbi` folders. These files are specific to a local Power BI Desktop session and are not required to open the project.
