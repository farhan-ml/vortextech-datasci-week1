# vortextech-datasci-week1

**Vortex Tech Data Science & Analytics Internship — Week 1 Submission**
Track: Beginner — Data Cleaning and Basic Visualization

## Description

A beginner-level data analytics project that walks through the full workflow of taking a messy real-world dataset (the Titanic passenger records) and turning it into clean, analysis-ready data with clear, well-labeled visualizations. Built as the Week 1 deliverable for the Vortex Tech Data Science & Analytics internship track.

**What it demonstrates:**
- Data inspection and cleaning with `pandas` (missing values, duplicates, data types)
- Exploratory data visualization with `matplotlib` and `seaborn`
- Clear documentation of reasoning at each step (markdown cells explain *why*, not just *what*)

## What This Is

This project takes the public **Titanic passenger dataset** (891 rows, mix of numeric and categorical columns), cleans it, and produces five visualizations that reveal patterns around survival, age, gender, and fare.

## Dataset

- **Source:** [seaborn-data / Titanic](https://github.com/mwaskom/seaborn-data) (public dataset, originally from Kaggle's Titanic competition)
- **Rows:** 891
- **Columns:** 15 (mix of numeric: `age`, `fare`, `sibsp`; categorical: `sex`, `class`, `embark_town`)

## What Was Done

1. Loaded the dataset and inspected structure with `.head()` / `.info()`
2. Identified and handled missing values:
   - `age` → filled with median
   - `deck` → dropped (77%+ missing)
   - `embarked` / `embark_town` → dropped 2 rows with missing values
3. Removed duplicate rows
4. Fixed data types (converted relevant columns to `category`)
5. Produced 5 visualizations with titles and axis labels:
   - Bar chart: Survival count by passenger class
   - Histogram: Age distribution
   - Pie chart: Gender split
   - Bar chart: Survival rate by gender
   - Line chart: Average fare by age group

## How to Run

```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook week1_data_cleaning.ipynb
```

Run all cells top to bottom. The notebook downloads/reads `titanic.csv` (included in this repo) and reproduces all cleaning steps and charts.

## Files

- `week1_data_cleaning.ipynb` — main notebook (cleaning + visualizations)
- `titanic.csv` — dataset used
- `requirements.txt` — Python dependencies
- `.gitignore` — files/folders excluded from version control
- `README.md` — this file

## Suggested GitHub Repo Topics

`data-science` `data-cleaning` `data-visualization` `pandas` `matplotlib` `seaborn` `jupyter-notebook` `internship` `vortextech`

## Author

Muhammad Farhan — Data Science & Analytics Intern, Vortex Tech (2026)
