# The Rhythm of a City — Bike Sharing Analysis

A Scientific Data Visualization project analyzing bike-sharing demand in Washington, D.C., using data from 2011–2012.

## Project Overview

The goal is to explore how time, weather, and user behavior are associated with bike-sharing demand.

The analysis includes:
- Data cleaning and preprocessing
- Exploratory data visualization
- Weather and seasonal analysis
- Statistical analysis
- K-Means clustering and daily mobility patterns

## Dataset

The dataset is available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset).

It contains:
- **17,379 hourly observations**
- **731 daily observations**
- Approximately **3.3 million bike rentals**

## Project Structure

```text
SCI-VIZ-PROG/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01_DataCleaning.ipynb
│   └── 02–08_Analysis.ipynb
└── output/
    └── figures/
```

## How to Run

1. Install the required Python libraries.
2. Open the notebooks using Jupyter Notebook or VS Code.
3. Run `01_DataCleaning.ipynb` to prepare the dataset.
4. Run notebooks `02–08` to generate the analyses and visualizations.

Generated figures are saved in `output/figures/`.

## Tools

Python, Pandas, NumPy, Matplotlib, Scikit-learn, and Jupyter Notebook.

## Limitations

The dataset covers only Washington, D.C., from 2011 to 2012. Some hourly observations are missing, and the analysis does not establish causal relationships.

## References

- [UCI Bike Sharing Dataset](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset)
