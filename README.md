# SC475 Time Series Analysis: Analyzing Fuel Price Trends in USA

## Abstract

In this study, we examine monthly datasets of US diesel and kerosene prices along with US railway and airline ticket prices from 2000 to 2020. We visualize trends, seasonality, and residual components through time-series decomposition and conduct statistical analyses including mean-variance evaluation, auto-covariance analysis, and stationarity tests.

We then explore:

* The relationship between diesel prices (\$/gal) and railway ticket prices.
* The relationship between kerosene prices (\$/gal) and flight ticket prices.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Folder Structure](#folder-structure)
3. [Data Description](#data-description)
4. [Code Walkthrough](#code-walkthrough)
5. [Installation & Requirements](#installation--requirements)
6. [Usage Instructions](#usage-instructions)
7. [Reports & Presentation](#reports--presentation)
8. [Results & Findings](#results--findings)
9. [Contributing](#contributing)


## Project Overview

This repository contains all materials for the SC475 Time Series Analysis project on fuel price trends in the USA and their implications for the airline and railway industries. You will find raw datasets, Python analysis notebooks, final report (IEEE format), and presentation slides.

## Folder Structure

```
├── Data_set/
│   ├── diesel_prices_us.csv
│   ├── kerosene_prices_us.csv
│   ├── railway_ticket_prices_us.csv
│   └── airline_ticket_prices_us.csv
│
├── Codes/
│   └── Analysis_on_Diesel&Railways.ipynb
|   └── Analysis_on_Kerosene&Flights.ipynb
│
├── Report/
│   ├── SC475_202201315_202201320.pdf
│   └── SC475_202201315_202201320_LaTeX.zip
│
└── PPT/
    └── SC475_202201315_202201320.pptx
```

1. **Data\_set**: Raw monthly data (2000–2020) with no errors.
2. **Codes**: Jupyter notebook (`.ipynb`) implementing the analysis.
3. **Report**: PDF and LaTeX source (IEEE standard).
4. **PPT**: 12‑slide presentation overview.

## Data Description

Each CSV in `Data_set/` contains:

* **Date**: Monthly timestamp (YYYY-MM).
* **Price**: Diesel or kerosene price in USD per gallon, or ticket price in USD.

All series cover January 2000 through December 2020.

## Code Walkthrough

Open `Codes/time_series_analysis.ipynb`. Key sections:

1. **Data Loading**
   Mount your Google Drive and load CSVs.
2. **Exploratory Data Analysis**
   Plot time series, summary statistics, distributions.
3. **Decomposition**
   Trend, seasonal, residual via STL/seasonal\_decompose.
4. **Statistical Tests**

   * Stationarity (ADF, KPSS tests)
   * Auto-covariance & correlograms
5. **Relationship Analysis**

   * Cross-correlation between diesel & railway price series.
   * Cross-correlation between kerosene & airline price series.
6. **Conclusions**
   Interpret economic and industry implications.

> **Note:** Modify only the cell that mounts the GDrive to point to your Data\_set folder. All other cells run end-to-end.

## Installation & Requirements

* Python 3.8+
* Jupyter Notebook or JupyterLab

Install dependencies:

```bash
pip install -r requirements.txt
```

**requirements.txt** should include:

```
pandas
numpy
matplotlib
statsmodels
seaborn
scipy
```

## Usage Instructions

1. Clone the repository:

   ```bash
   ```

git clone  cd&#x20;

````
2. Place `Data_set/` in your Google Drive root (or adjust mount path in notebook).
3. Launch Jupyter Notebook:
   ```bash
jupyter notebook Codes/time_series_analysis.ipynb
````

4. Run all cells sequentially.

## Reports & Presentation

* **Final Report**: `Report/SC475_202201315_202201320.pdf` (IEEE format).
* **LaTeX Source**: `Report/SC475_202201315_202201320_LaTeX.zip`.
* **Presentation**: `PPT/SC475_202201315_202201320.pptx` (12 slides).

## Results & Findings

* Diesel prices and railway ticket prices exhibit a moderate positive correlation (lag 0–3 months), suggesting fuel cost pass-through to fares.
* Kerosene prices lead airline ticket prices by \~2 months, indicating pricing adjustments with a lag.
* Seasonal patterns strong in both industries—peak travel seasons amplify price sensitivity.

*For detailed tables, figures, and statistical test results, see the notebook and report.*

## Contributing

This project is maintained by:

- **[Jal Dani](https://github.com/JalDani2010)** – Primary author and analyst  
- **[Sumit Vishwakarma](https://github.com/Sumit-320)** – Primary author and analyst





