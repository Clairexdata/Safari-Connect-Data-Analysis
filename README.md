# Safari Connect Operations

A transport operations analysis project using PostgreSQL for data cleaning and analysis and Power BI for reporting.

## Overview

The dataset contains 288 bookings across 10 routes and 8 drivers. The analysis examines route revenue, driver and passenger ratings, monthly trends, cancellations, payment methods, and operating patterns.

## Highlights

- 253 completed trips earned **KES 227,810**; 35 cancellations or no-shows represented **KES 32,150** in lost booked value.
- RT001 (Nairobi–Mombasa) earned the most: **KES 51,600**. RT005 had the most bookings, but earned KES 7,620.
- Wednesday had the most bookings; Monday earned the most revenue.
- Average passenger satisfaction was **3.53/5**. Cash bookings had the highest failure rate (**21.6%**).
- H2 2024 revenue was **16.8%** higher than H1.

## Files

- `safari_connect_clean.csv` — cleaned booking data
- `SAFARI_CONNECT_DATA_ANALYSIS_SCRIPT.txt` — SQL analysis and validation queries
- `Safari Connect -Operational Dashboard_.pdf` — static dashboard export
- `SafariConnect_Dashboard_Brief.docx` — findings and dashboard notes

## Reproduce

Load the data into PostgreSQL, make it available as `v_clean_trips.safari_connect_clean`, then run the SQL analysis script. Open the `.pbix` file in Power BI Desktop and configure its database connection.

## Limitations and privacy

Revenue is not profit because cost data is unavailable. January 2025 is excluded from monthly comparisons because it contains only three bookings through 4 January. The CSV includes passenger names and phone numbers; remove or anonymize personal data before publishing it publicly.
