
# Assignment 1  Overview
This assignment performs data cleaning on a emergency triage dataset as part of an introductory data preprocessing assignment. The focus is exclusively on the Gender column, which contains inconsistent categorical representations (Male, MALE, 1, Female, FEMALE, 0). The goal is to standardize these values into a clean binary numeric format (1 for male, 0 for female).

# What Was Done
1. Load the data from Google Drive (the notebook assumes the file is stored in a specific Colab path).

2. Inspect the Gender column – check unique values and value counts to understand the inconsistencies.

3. Create a mapping dictionary that translates every observed variant:

    'Male', 'MALE', '1' → 1

    'Female', 'FEMALE', '0' → 0

4. Apply the mapping to produce a new clean column Gender_Clean.

5. Drop the original Gender column and rename Gender_Clean → Gender.

6. Verify the result (no missing values, only 0/1, correct counts).

# Libraries used:
  Pandas
  
  Numpy

  matplotlib
