# Supplier Risk Analysis & Freight Logistics Optimization Pipeline

**Focus:** Supplier reliability, lead-time variation, freight delays and OTIF  
**Tools named in resume:** Tableau, SQL, window functions, CTEs, Python, SAP SCM data and Excel VBA.

## Business question

Which suppliers, lanes or purchase orders deserve attention first because of late delivery patterns, variable lead times or price variance?

## Analytical workflow

1. Standardize supplier, purchase-order, promised-date, receipt-date, quantity and unit-price fields.
2. Calculate delivery lateness and lead-time variability at PO and supplier level.
3. Define OTIF precisely: a delivery counts only when it is both on time and in full, using an agreed tolerance and date definition.
4. Compare actual lead time with contracted or planned lead time.
5. Identify high-risk suppliers and freight lanes using transparent, explainable rules.
6. Present exceptions, trends and supplier comparisons in a Tableau dashboard.

## Example KPIs

- OTIF rate = on-time and in-full eligible deliveries / total eligible deliveries.
- Average and median lead time.
- Lead-time standard deviation or coefficient of variation.
- Late PO count and overdue open-PO value.
- Unit-price variance against an approved reference price.

## Resume-reported project outcome

The supplied resume describes analysis of **50+ vendor lead times**, carrier delays and pricing variances, with a reported **14% improvement in OTIF delivery compliance**. Add the baseline, time period, population, and calculation method before publishing this as a measured result.

## Suggested public demo

Build a synthetic supplier/PO dataset. Include SQL examples for late-PO ranking, rolling supplier OTIF, lead-time variability and price variance. Use a Tableau Public workbook or screenshots based only on the synthetic data.

> **Data note:** This is a project case-study outline based on the supplied resume. It is not a claim that employer-confidential datasets or dashboards are included in this public repository.
