# Copilot Instructions for AI Coding Agents

## Project Overview
This project is a collection of Jupyter notebooks for statistical analysis using the possum dataset (`possum.csv`). The focus is on measures of central tendency, measures of spread, and outlier detection, with all code and analysis performed in Python using pandas, numpy, matplotlib, seaborn, and scipy.

## Key Files and Structure
- `possum.csv`: Main dataset for all analyses.
- `task18_possum.ipynb`, `task1_mmm.ipynb`, etc.: Jupyter notebooks for different statistical tasks and explorations.

## Patterns and Conventions
- Data is always loaded from `possum.csv` using pandas (`pd.read_csv`).
- Data cleaning (handling missing values, resetting index, removing duplicates) is performed at the start of each notebook.
- Use `select_dtypes` to separate categorical and numerical columns.
- Descriptive statistics for categorical columns use `describe(include='all')` and custom summary functions.
- Descriptive statistics for numerical columns use `describe()`, `.mean()`, `.median()`, `.mode()`, `.std()`, etc.
- Visualizations (if present) use matplotlib and seaborn.
- All code is written in Python 3, and notebooks may use `%pip install` for dependencies.

## Developer Workflows
- Notebooks are the primary development and analysis environment.
- To add new analysis, create a new notebook or extend an existing one, following the established data loading and cleaning steps.
- No custom build or test scripts are present; validation is by running notebook cells.

## Integration and Dependencies
- All dependencies are standard Python data science libraries: pandas, numpy, matplotlib, seaborn, scipy, statistics.
- No external APIs or services are integrated.

## Examples
- See `task18_possum.ipynb` for examples of data cleaning, summary statistics, and custom functions for categorical data analysis.
- Use `groupby` and `describe` for grouped statistics (e.g., `possum_data.groupby('sex')['age'].describe()`).

## Special Notes
- Follow the pattern of cleaning data before analysis.
- When adding new statistical methods, document the interpretation of results in markdown cells.
- Keep code and markdown well-separated for clarity.

---
For questions or unclear conventions, review the most recent notebook (`task18_possum.ipynb`) for up-to-date patterns.
