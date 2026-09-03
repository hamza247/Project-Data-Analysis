# Exploratory Data Analysis - Automobile Dataset

## Project Overview

This project is an Exploratory Data Analysis (EDA) of an automobile dataset.

The purpose of the project is to clean, explore, analyse, and visualise automobile data in order to identify useful patterns and relationships between vehicle characteristics such as price, engine size, horsepower, fuel efficiency, and manufacturer.

The project was completed using Python in a Jupyter Notebook.

---

## Dataset

The dataset used in this project is:

`automobile.txt`

The original dataset contains:

- 205 rows
- 26 columns

The dataset contains information about different automobiles, including:

- Manufacturer
- Body style
- Fuel type
- Engine size
- Horsepower
- City MPG
- Highway MPG
- Price
- Number of cylinders
- Vehicle dimensions

Some missing values in the original dataset are represented by `?`.

---

## Project Objectives

The main objectives of this project were to:

1. Load and inspect the automobile dataset.
2. Clean the dataset.
3. Remove unnecessary columns.
4. Check for and remove duplicate records.
5. Identify and remove rows containing missing values.
6. Convert appropriate numerical columns to the correct data types.
7. Create a DataFrame containing hatchback automobiles.
8. Investigate the five most expensive automobiles.
9. Compare expensive and inexpensive automobiles.
10. Identify the most fuel-efficient manufacturer.
11. Find automobiles with the largest engine capacity.
12. Identify the manufacturer with the most vehicle records.
13. Create clear visualisations to support the analysis.
14. Summarise the main findings in an EDA report.

---

## Data Cleaning

Several data-cleaning steps were performed before the analysis.

### Removed Columns

The following columns were removed because they were not required for the analysis:

- `normalized-losses`
- `symboling`

### Duplicate Records

The dataset was checked for duplicate rows using Pandas.

Duplicate rows were removed using:

```python
automobiles_df.drop_duplicates()
