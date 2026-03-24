# Lightning Strike Analysis (2018): NOAA Data Exploration

## Project Overview
This project analyzes more than 3.4 million NOAA lightning records from 2018 to identify daily and seasonal strike patterns.  
The workflow demonstrates data cleaning, feature engineering, aggregation, and visualization implemented using Python in a Jupyter notebook environment.  
Results show clear summer concentration, with August being the peak month.

## Project Background
The NOAA monitors atmospheric activity, including lightning, using satellite-based systems such as the GOES satellites equipped with Geostationary Lightning Mapper (GLM) technology. 

This project focuses on understanding how lightning activity changed over time across 2018.

## Project Goal
Use Python in Jupyter Notebook to:
- prepare and validate NOAA lightning data,
- calculate total lightning strikes by day and month,
- visualize monthly trends.

## Dataset
- **Source file:** `lightning_strikes_1.csv`
- **Size:** 3,401,012 rows, 3 columns
- **Columns:**
  - `date` (string, converted to datetime)
  - `number_of_strikes` (integer)
  - `center_point_geom` (geospatial point text)

## Tools and Libraries
- Python
- Jupyter Notebook
- pandas
- numpy
- datetime
- matplotlib

## Method
1. Load and inspect dataset with `head()`, `shape`, and `info()`.
2. Convert `date` to datetime format.
3. Create a `month` feature from `date`.
4. Aggregate total strikes by day and rank highest-activity days.
5. Aggregate total strikes by month.
6. Build a monthly bar chart (`month_txt` vs `number_of_strikes`).

## Key Findings
- Lightning activity peaks strongly in summer months.
- **August** had the highest monthly total with **15,525,255** strikes.
- Top daily strike counts were concentrated in August (for example, August 29 had 1,070,457 strikes).

## Visualization Summary
The monthly bar chart shows a gradual rise from spring into summer, a sharp peak in August, and then a steady decline through fall and winter,
signaling a strong seasonal behavior in 2018 lightning strikes.

## Notes
- The full dataset is not included in the repo due to size, A truncated sample is used for demonstration.

## Source
- Project reference: https://shadyeggs.github.io/2018-NOAA-Lightning-Strike-Data/
- Data origin: NOAA lightning observations (2018)
