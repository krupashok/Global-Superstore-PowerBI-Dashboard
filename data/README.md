# Dataset documentation

## File

`Global_Superstore.csv` contains 51,290 fictional retail transaction rows and 27 columns.

## Fields

| Group | Columns |
|---|---|
| Order and customer | `Row ID`, `Order ID`, `Customer ID`, `Customer Name`, `Segment`, `Order Priority` |
| Product | `Product ID`, `Product Name`, `Category`, `Sub-Category` |
| Geography | `City`, `State`, `Country`, `Region`, `Market`, `Market2` |
| Commercial measures | `Sales`, `Profit`, `Quantity`, `Discount`, `Shipping Cost` |
| Fulfilment | `Ship Mode`, `Order Date`, `Ship Date` |
| Time and helper fields | `Year`, `weeknum`, `ji_lu-shu` |

## Full-file audit

| Check | Result |
|---|---:|
| Rows | 51,290 |
| Columns | 27 |
| Blank cells | 0 |
| Distinct order IDs | 25,035 |
| Distinct customer IDs | 4,873 |
| Countries | 147 |
| Sales total | 12,642,905.00 |
| Profit total | 1,467,457.2913 |
| Quantity total | 178,312 |
| Shipping cost total | 1,352,815.7034 |

## Known limitation

The supplied `Order Date` and `Ship Date` values are all `00:00.0`, which means the original full dates cannot be reconstructed from this export. Use `Year` and `weeknum` for supported time analysis, or replace the date fields with a verified source dataset before extending the report to daily or monthly trends.

## Privacy and provenance

This is fictional sample retail data used for analysis practice. A scan found no email addresses, API keys, passwords, or other obvious credentials. The customer names and IDs are retained because they are part of the fictional sample and support order-level analysis.

The CSV appears to be a transformed Global Superstore sample export. Original dataset rights remain with the source; no separate dataset licence is granted by this repository.
