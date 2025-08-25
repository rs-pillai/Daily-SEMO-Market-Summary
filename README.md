# Daily-SEMO-Market-Summary
This repository contains scripts and workflows to automatically gather, clean, and process SEMOpx (Single Electricity Market Operator power exchange) data.   The project focuses on retrieving daily market results, structuring them for analysis, and ensuring reproducibility of data pipelines used in electricity market modelling.
## Objectives

- Automate the download and organisation of **daily SEMOpx market data** (Day-Ahead, Intraday, Balancing where applicable).  
- Parse and transform SEMOpx-provided files into structured **CSV/JSON formats** for further analysis.  
- Handle pagination, date selection, and data quality checks in an automated manner.  
- Store processed outputs for use in **market modelling and forecasting workflows**.  

---

## Methods (Summary)

1. **Data Retrieval**  
   - Queries SEMOpx APIs or published datasets.  
   - Handles request pagination and dynamic URLs for different dates.  

2. **Data Processing**  
   - Extracts relevant fields (timestamps, delivery date, market type, price, volumes).  
   - Ensures consistent formatting (ISO datetimes, numeric types).  
   - Validates completeness (e.g., all 24 hours/day available).  

3. **Outputs**  
   - Cleaned datasets stored as CSV in a structured folder.  
   - Optionally stores metadata/logs for auditing.
  
## Results

The workflow generates:

- **Daily CSV files** containing SEMOpx market data (Day-Ahead and other products).  
- **Aggregated tables** with hourly market clearing prices and traded volumes.  
- **Logs/metadata** for troubleshooting and auditing the data pipeline.  

All results are stored in the `results/` directory.

---

## Data Availability

- Data originates from the **SEMOpx public market data portal**.  
- The raw files are publicly available, but this repository provides **scripts** to automate retrieval and processing.  
- Cleaned outputs included here are for demonstration purposes; users should re-run the pipeline for up-to-date market data.


## Contact

   Rahul Sajith Pillai
   
   PhD Researcher - Ulster University, Belfast
   
   Email: pillai-rs@ulster.ac.uk

   [LinkedIn](https://www.linkedin.com/in/rahul-sajith-p-02a7b6a3)

