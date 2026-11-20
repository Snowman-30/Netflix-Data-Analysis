# Netflix Data Analysis

An exploratory data analysis (EDA) project investigating the content available on Netflix, using Python, Pandas, NumPy, and Matplotlib.

> **Project status:** In progress. The analysis is being developed step by step, with data-quality checks, cleaning, and exploratory questions documented in the Jupyter Notebook.

## Overview

This project explores the Netflix titles dataset to understand the composition of its catalogue and how content additions vary over time. The work focuses on inspecting the dataset, identifying data-quality issues, cleaning selected fields, and answering analytical questions with Python.

The project is intended to demonstrate a practical data-analysis workflow: inspect the data, assess its quality, prepare it for analysis, investigate meaningful questions, and communicate findings.

## Dataset

- **File:** `netflix_titles.csv`
- **Records:** 8,807 titles
- **Columns:** 12
- **Main fields:** show ID, content type, title, director, cast, country, date added, release year, rating, duration, genres/categories, and description.

The dataset contains information about movies and TV shows available on Netflix. Please refer to the original dataset source and its licence/terms before redistributing or reusing the data.

## Tools and Technologies

- **Python** — analysis language
- **Jupyter Notebook** — interactive analysis and documentation
- **Pandas** — data inspection, cleaning, and manipulation
- **NumPy** — numerical operations
- **Matplotlib** — data visualization (used for visual analysis as the project develops)
- **Git and GitHub** — version control and project hosting

## Project Structure

```text
Netflix-Data-Analysis/
├── netflix_titles.csv       # Dataset used for the analysis
├── Netflix Analysis.ipynb   # Jupyter Notebook containing the analysis
├── README.md                # Project documentation
├── .gitignore               # Files and folders excluded from Git
└── .gitattributes           # Git text and file-handling settings
```

## Work Completed So Far

### 1. Initial Data Inspection
- Loaded the CSV dataset with Pandas.
- Reviewed its dimensions, columns, data types, and missing-value counts.
- Checked the uniqueness of show IDs and titles.
- Investigated duplicate rows.

### 2. Data Quality Assessment and Cleaning
- Examined missing values across columns.
- Investigated records with missing dates and other incomplete fields.
- Identified three duration-like values stored incorrectly in the `rating` column (`74 min`, `84 min`, and `66 min`).
- Moved those values into the `duration` column and marked the incorrect rating entries as missing.
- Converted `date_added` into a datetime field for time-based analysis.

### 3. Exploratory Analysis
- Compared the number and proportion of Movies and TV Shows.
- Grouped release years into decades to examine the distribution of titles by release period.
- Examined how many titles were added to Netflix in each year.
- Compared title additions across earlier and later periods.
- Calculated year-to-year changes in the number of titles added.

## Questions Explored

The notebook currently investigates questions such as:

1. How many Movies and TV Shows are included in the dataset, and what share does each represent?
2. How are titles distributed across release decades?
3. How many titles were added to Netflix each year?
4. How did Netflix title additions differ between earlier and later periods?
5. Which years experienced the largest increases or decreases in additions?

Further questions, visualizations, and conclusions will be added as the analysis progresses.

## Current Findings

- The dataset contains **8,807 titles**.
- It includes **6,131 Movies (69.6%)** and **2,676 TV Shows (30.4%)**.
- Movies make up the larger share of the records in this dataset.

These figures describe the dataset being analysed; they should not be interpreted as a live count of Netflix's current catalogue.

## How to Run the Project

1. Clone or download this repository.
2. Make sure Python and Jupyter Notebook are installed.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib jupyter
   ```

4. Keep `netflix_titles.csv` in the same directory as the notebook.
5. Open Jupyter Notebook and run `Netflix Analysis.ipynb`:

   ```bash
   jupyter notebook
   ```

## Repository Contents

- [Netflix Analysis Notebook](Netflix%20Analysis.ipynb)
- [Netflix Titles Dataset](netflix_titles.csv)

## Next Steps

- Continue exploring country-wise and genre-wise content patterns.
- Add clear, well-labelled visualizations to support the analysis.
- Investigate trends by content type and year.
- Summarize the most useful insights and limitations.
- Refine the notebook and documentation as the project is completed.

## Notes

This is a learning and portfolio project. The notebook records the analysis as it develops, including exploratory work. Results and interpretations may be refined as additional validation and analysis are completed.
