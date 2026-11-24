# End-to-End Demand Forecast Engine & Inventory Control Tower

**Focus:** Demand forecasting, replenishment signals and inventory visibility  
**Tools named in resume:** Python, Pandas, statsmodels, Prophet, Advanced SQL, Power BI, DAX, PostgreSQL and Excel.

## Business question

How can a planning team turn historical order patterns into a repeatable forecast and inventory review process, while making stockout exposure and replenishment priorities easier to see?

## Workflow

1. **Prepare the data:** validate order dates, product identifiers, quantities, missing values and duplicate records.
2. **Explore demand:** profile demand by SKU and time period; inspect trend, seasonality, outliers and intermittent demand.
3. **Build a baseline:** compare a naïve or seasonal-naïve forecast with an ARIMA model and (where suitable) Prophet.
4. **Back-test:** use a time-based holdout rather than random train/test splitting. Compare MAE, RMSE and MAPE / WAPE, with care around zero-demand periods.
5. **Translate forecast to planning signals:** combine forecast demand, lead time, review period, on-hand inventory and open supply to calculate projected coverage and reorder alerts.
6. **Visualize:** design a Power BI control-tower view for forecast error, inventory status, safety-stock exceptions and replenishment priorities.

## Example measures

- Forecast error: MAE, RMSE, WAPE / MAPE (document the denominator and treatment of zero demand).
- Inventory cover: available inventory divided by average daily demand.
- Reorder trigger: demand during lead time plus an explicitly documented safety-stock assumption.
- Stockout exposure: projected demand not covered by available and expected supply.

## Resume-reported project outcome

The supplied resume describes processing **100K+ historical order records** and reducing inventory stockout risk by **28%**. Treat these as resume-reported results; add the measurement period, baseline, definition of stockout risk and validation evidence before presenting them as independently reproducible outcomes.

## Public demonstration plan

Create a synthetic dataset with columns such as `order_date`, `sku_id`, `quantity`, `location_id`, `lead_time_days`, `on_hand_qty` and `open_po_qty`. Use generated sample records only. Add a notebook showing data validation, train/test split, baseline comparison, model evaluation and a replenishment exception table.

> **Data note:** This repository currently contains the case-study specification, not employer source data or a verified implementation. Any future demo dataset must be clearly labelled synthetic. Never publish proprietary or personally identifiable data.
