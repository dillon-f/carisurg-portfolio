# Carisurg – Emergency Triage Data Cleaning, Visualisation, and Triage Modelling

## Project Overview

This repository contains a series of assignments and tutorials focused on **emergency department triage data**. The work includes:

- Cleaning a dirty emergency triage dataset
- Visualising key vital signs to answer clinical questions
- Recommending an additional vital sign (SpO₂)
- Developing pseudocode for a rule‑based digital triage system
- Time Management and Career challenges

All code is written in Python using Jupyter notebooks, with libraries such as pandas, numpy, and matplotlib.

## Dataset

- **Original file:** `EmergencyTriageDataset_Reduced_Dirty.csv`
- **Rows:** 2,205
- **Columns:** ID, Age, Gender, GCS, SBP, DBP, MAP, pulse, Temp, RR, Fio2

The dataset contains realistic clinical measurements (with intentional errors and missing values) that were cleaned in the assignments.

## Repository Contents

| File / Notebook | Description |
|----------------|-------------|
| `Assignment 1.ipynb` | Cleaning the **Gender** column (inconsistent values → binary numeric). |
| `Assignment2_DataCleaningFiO2_AssignedColumn_Group.ipynb` | Cleaning the **FiO₂** column, including mode imputation for missing values. |
| `Tutorial_3_(week0)_Visualisation.ipynb` | Full data cleaning (all columns) + visualisations: SBP histogram and Age‑vs‑SBP scatter plot. |
| `Assignment 4 - Vital Sign Description` | Description of **Systolic Blood Pressure (SBP)** – definition, clinical ranges, triage importance. |
| `Assignment 5 - Unconsidered Metrics` | Recommendation of **Peripheral Oxygen Saturation (SpO₂)** as an additional vital sign, including limitations. |
| `Assignment 6- Pseudocode` | **Pseudocode** for a digital triage system using the dataset’s vital signs (GCS, SBP, DBP, MAP, pulse, Temp, RR, FiO₂). |
| `Assignment 7- Career challenges` | **Career Challenges** |


## Key Achievements

### Data Cleaning
- Standardised **Gender** from 6 variants to binary (1 = male, 0 = female).
  
### Full Dataset Cleaning 
- Imputed **FiO₂** missing values using the **mode (21%)** because FiO₂ is a discrete clinical setting.
- Converted all vitals to numeric, applied physiological ranges, and imputed missing values ( mode for FiO₂).
- Final dataset: 2,205 rows × 11 columns, **no missing values**.

### Visualisation 
- **Histogram of SBP** with clinical reference lines (hypotension, ideal, pre‑hypertension, hypertensive crisis).
- **Scatter plot of Age vs SBP** to answer: *Does systolic blood pressure increase with age?* – weak positive association observed.

### Additional Vital Sign 
- Recommended **SpO₂** (oxygen saturation). Clinical ranges: 95‑100% normal, 90‑94% mild hypoxia, 85‑89% moderate, <85% severe.
- Noted limitations: cold hands, nail polish, carbon monoxide poisoning.

### Triage Pseudocode
- Rule‑based algorithm assigning categories 1 (immediate) to 5 (non‑urgent).
- Uses thresholds for GCS, SBP, DBP, MAP, pulse, RR, Temp, FiO₂, and chief complaint keywords.

## Technologies Used

- Python 3
- pandas, numpy, matplotlib
- Jupyter Notebook / Google Colab
- Git & GitHub

## How to Navigate

- Each assignment/tutorial is a separate notebook or Markdown file.
- Open the notebooks in order (Assignment 1 → Assignment 2 → Assignment 3) to follow the progression from cleaning to visualisation.
- The `README.md` files for all Assignments contain standalone summaries.


