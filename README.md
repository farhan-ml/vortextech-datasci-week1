# VortexTech Week 1 — Data Cleaning and Basic Visualization

## What I built
A Jupyter Notebook that cleans the Titanic passenger dataset (891 rows, from Kaggle) and
produces 5 visualizations exploring survival patterns.

## What's in the notebook
- Loading and initial inspection of the dataset (`.head()`, `.info()`, `.columns`)
- Handling missing values:
  - `Age` (177 missing) — filled with the median
  - `Cabin` (687 missing, >75%) — column dropped
  - `Embarked` (2 missing) — filled with the mode
- Removing duplicate rows
- Fixing data types (converting `Survived`, `Pclass`, `Sex`, `Embarked` to categorical)
- 5 visualizations with titles, axis labels, and markdown explanations:
  1. Age distribution (histogram)
  2. Passenger count by class (bar chart)
  3. Survival count by sex (bar chart)
  4. Overall survival rate (pie chart)
  5. Survival rate by age group (line chart)

## How to run it
1. Install dependencies: `pip install pandas matplotlib seaborn jupyter`
2. Make sure `titanic.csv` is in the same folder as the notebook
3. Open the notebook: `jupyter notebook week1_updated.ipynb`
4. Run all cells

## Dataset
Titanic passenger dataset from Kaggle: https://www.kaggle.com/c/titanic/data
