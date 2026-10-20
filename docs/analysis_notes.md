# Analysis notes and business questions

## Questions the workbook is designed to explore

1. How do total sales, line counts, and average sales per line change over time?
2. Which product classes and channels contribute most to sales?
3. How concentrated are sales among distributors?
4. How does the geographic mix change across years?
5. Which sales teams and representatives contribute most?
6. Where are negative values or potential duplicate records that need review?

## Findings from the supplied CSV

- **Overall sales:** approximately 11.80 billion in the source's numeric units. The currency is not specified.
- **Year with highest sales:** 2018, approximately 3.51 billion. It has 94,434 rows, compared with about 51,000–56,000 rows in each other year. Total sales should therefore be considered alongside record volume and average sales per row.
- **Geographic mix:** Germany contributes about 94.2% of net sales; Poland contributes the remainder. Poland appears only in 2018, so cross-country year-over-year comparisons are not like-for-like.
- **Channel mix:** Pharmacy contributes about 52.7% and Hospital about 47.3% of net sales.
- **Largest product class:** Analgesics, at about 2.37 billion.
- **Negative sales:** 2,633 rows (about 1.04%) have negative `Sales`. They could be returns, credits, corrections, or data problems. The dataset alone cannot establish which explanation is correct.
- **Distributor concentration:** the top 10 distributors account for about 92.6% of net sales. Confirm the business meaning of distributor names and the completeness of the data before drawing operational conclusions.
- **Concentration in large records:** the largest 1% of rows account for about 40.4% of net sales. Validate large values and whether row-level totals represent comparable transaction units.

## Recommended next checks

- Confirm data provenance, licensing, and whether names are anonymized.
- Confirm the currency and the meaning of `Price`, `Quantity`, and negative `Sales`.
- Check whether rows represent transaction lines, aggregated sales lines, or another unit.
- Investigate possible duplicates before removing any records.
- Verify all workbook filters, navigation, and dashboard interactions in Tableau Desktop.
