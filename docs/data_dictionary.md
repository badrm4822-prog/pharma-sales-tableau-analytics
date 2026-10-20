# Data dictionary

The packaged workbook contains an extract of the supplied pharmaceutical sales dataset. The field descriptions below are inferred from the column names and sample rows; verify business definitions with the data owner.

| Field | Description |
|---|---|
| `Distributor` | Distributor name associated with the sales record. |
| `Customer Name` | Customer/account name. |
| `City` | City associated with the record. |
| `Country` | Country associated with the record. |
| `Latitude` | Geographic latitude. |
| `Longitude` | Geographic longitude. |
| `Channel` | Primary sales channel (for example, Pharmacy or Hospital). |
| `Sub-channel` | More specific channel category (for example, Retail or Private). |
| `Product Name` | Product/medicine name. |
| `Product Class` | Product therapeutic/category classification as provided. |
| `Quantity` | Quantity recorded for the transaction line. |
| `Price` | Unit price field in the source; currency is not specified. |
| `Sales` | Sales amount recorded for the transaction line; currency is not specified. |
| `Month` | Month label. |
| `Year` | Year of the record. |
| `Name of Sales Rep` | Sales representative name. |
| `Manager` | Manager name. |
| `Sales Team` | Sales team label. |

## Important caveats

- The source does not specify currency, unit conventions, or formal business definitions.
- Negative sales values are present; do not automatically classify them as errors without business context.
- Customer, distributor, and employee names may be sensitive. Check permission and privacy requirements before sharing the workbook publicly.
