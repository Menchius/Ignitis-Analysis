# AlphaWind – Asset Performance Investigation

## Project Overview

This project investigates the operational performance of
AlphaWind, a wind park consisting of six turbines, over a
seven-day period.

The objective is to identify the main drivers of energy
production losses, estimate expected production based on
wind conditions, investigate turbine-level performance
and evaluate the reliability of operational event records.

## Repository Structure

- `alphawind_investigation_final.ipynb` – Complete analytical
  investigation and Python implementation.
- `production.csv` – Turbine-level energy production.
- `weather.csv` – Park-level wind speed measurements.
- `stops_log.csv` – Operational event records.
- `turbine_metadata.csv` – Turbine information and service history.
- `outputs/` – Exported analytical results and visualizations.
- `stakeholder_brief.md` – Executive summary and operational
  recommendations.
- `requirements.txt` – Python dependencies.

## Methodology

The investigation includes:

1. Data inspection and quality assessment.
2. Exploratory analysis of park and turbine performance.
3. Development of an empirical expected-production baseline.
4. Operational event cleaning and reconciliation.
5. Identification of unlogged production derating.
6. Energy loss estimation and attribution.
7. Operational recommendations.

Expected production is estimated using a peer-based production
curve constructed from five reference turbines, excluding T04.

## Key Findings

- Actual production: 642.33 MWh.
- Estimated potential production: 726.99 MWh.
- Total theoretical production shortfall: 84.66 MWh.
- Operational shortfall excluding high-wind cut-out: 48.87 MWh.
- Main turbine-level concern: persistent underperformance of T04.
- Main operational concern: grid limitations and production losses
  concentrated on 6 March.

## Reproducing the Analysis

1. Clone this repository.
2. Install the required Python packages.
3. Open `alphawind_investigation_final.ipynb` in Jupyter Notebook.
4. Run all cells sequentially.

The notebook uses relative file paths and expects the original
CSV files to be located in the repository root.

## Limitations

The expected-production baseline is based on seven days of
observations and should be interpreted as an empirical
peer-based benchmark rather than a manufacturer-certified
power curve.
