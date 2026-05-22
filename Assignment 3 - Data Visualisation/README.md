# PROjECT OVERVIEW:

This assignment focuses on visualising the cleaned emergency triage dataset to answer a specific clinical question. Two plots are generated:

Histogram of Systolic Blood Pressure (SBP) – to understand the distribution of SBP values and identify patients in different clinical categories.

Scatter plot of Age vs SBP – to explore the relationship between patient age and systolic blood pressure.

The dataset used is fully cleaned (no missing values) after applying all previous data cleaning steps (Gender, GCS, SBP, DBP, pulse, temperature, RR, FiO₂, MAP).

# Clinical Question
Does systolic blood pressure increase with age in patients?

This question examines whether the known physiological trend (increased arterial stiffness and higher SBP with age) is observed in this triage population.

# Reference Lines and Annotations (Clinical Meaning)

Histogram of SBP
Blue dashed line at 90 mmHg – hypotension threshold (SBP < 90).

Green dashed line at 120 mmHg – upper bound of ideal range.

Green shaded area (90–120 mmHg) – ideal blood pressure range.

Orange dashed line at 139 mmHg – pre‑hypertension.

Red dashed line at 180 mmHg – hypertensive crisis threshold.

Scatter Plot (Age vs SBP)
Blue dashed horizontal line at 90 mmHg – hypotension threshold.

Orange dashed horizontal line at 140 mmHg – hypertension threshold (≥140 mmHg).

These reference lines allow immediate clinical interpretation: patients above the 140 line are hypertensive; those below 90 are hypotensive; the scatter plot also shows age‑related trends.

# Key Findings
SBP Distribution – Most patients have SBP in the ideal (90–120) or pre‑hypertensive (120–139) range. Few patients are hypotensive (<90), and a notable number have SBP ≥140 (hypertension). Very few reach hypertensive crisis (≥180).

Age vs SBP Relationship – There is a weak positive association between age and SBP. Older patients tend to have slightly higher SBP on average, but the scatter shows wide variability. Hypertension is present in all age groups, not exclusively in the elderly.

Hypotension is rare and occurs across all ages.

# Libraries Used
pandas 

numpy 

matplotlib.pyplot 
