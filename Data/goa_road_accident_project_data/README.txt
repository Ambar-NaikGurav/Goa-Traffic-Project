GOA ROAD ACCIDENT DATA — OFFICIAL SOURCE EXTRACTION

These CSVs are derived from the uploaded Goa Police monthly accident reports.

Datasets:
1. monthly_station_accidents.csv — police-station/month accident and fatality data.
2. goa_accident_scenario.csv — statewide Accident Scenario indicators.
3. data_dictionary.csv — field definitions.
4. validation_summary.csv — extraction checks.

Rules:
- Explicit 00 in a source table is stored as 0.
- An unreported station/month is left absent; it is NOT converted to zero.
- Colvala is retained in source_station_name and standardized to Colvale for analysis joins.
- YTD fields are cumulative and must not be treated as monthly counts.
- Comparison-year values are preserved as reported.

Coverage of supplied reports:
2025: February, April, July, August, September, October, November, December.
2026: February, March, May, June.
This is therefore not a complete month-by-month series for all months of 2025–2026.
