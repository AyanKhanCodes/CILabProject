# Global Tech Layoff Trends (2020-2025)

## Project Overview
This project is a data analytics dashboard designed to visualize the recent economic downturn in the global technology sector. Using a dataset spanning 2020 to 2025, the dashboard analyzes workforce reduction trends across various industries, geographic locations, and timeframes.

The primary objective was to move beyond high-level statistics and identify specific patterns, such as the correlation between post-pandemic economic shifts and the spike in layoffs during 2023.

## Key Findings
* **Scale of Impact:** The data indicates that over 826,000 employees across 2,852 unique companies have been affected during the analysis period.
* **Temporal Trends:** While 2020 saw initial instability due to COVID-19, the most significant workforce reductions occurred in a sharp, exponential spike starting in late 2022 and peaking in 2023.
* **Sector Analysis:** Consumer-facing industries (Retail, Consumer Tech) demonstrated higher vulnerability compared to sectors like Healthcare or Crypto, likely due to shifts in consumer spending power.
* **Geographic Distribution:** The United States remains the primary hotspot, but significant clusters were identified in major global tech hubs including Bangalore, London, and Berlin.

## Technical Implementation

### Tech Stack
* **Tool:** Power BI Service (Web Version)
* **Data Source:** Kaggle (Layoffs Dataset)
* **Data Processing:** ETL via Power Query (Online)

### Methodology & Constraints
Since this project was developed in a macOS environment, I utilized the **Power BI Service (Web)** instead of the Desktop application. This required adapting to the "Quick Create" interface and performing data modeling directly within the cloud environment.

### Data Modeling & DAX Measures
To ensure accurate reporting, I avoided default aggregations for certain fields and instead created specific measures:

1.  **Total Layoffs:**
    * Logic: `SUM(total_laid_off)`
    * Purpose: Calculates the total volume of affected employees.

2.  **Company Count:**
    * Logic: `DISTINCTCOUNT(company)`
    * Purpose: The dataset contained multiple entries for companies that had several rounds of layoffs. A distinct count was necessary to determine the actual number of unique organizations impacted, preventing data duplication.

## Author
**Ayan Khan** **23FE10CSE00504**
*Focus: Data Visualization, Business Intelligence*
