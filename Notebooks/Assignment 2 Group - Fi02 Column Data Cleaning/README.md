# Overview
This assignment focuses exclusively on cleaning the FiO2 (Fraction of Inspired Oxygen) column in the emergency triage dataset. The goal is to inspect, validate, visualise, and impute missing values in a clinically appropriate manner. 

# Data Exploration
Before any cleaning, the FiO₂ column was examined to understand its structure and quality. 
Unique values were observed and a total of 22 missing values (NaN) were identified. The minimum value present was 21.0 and the maximum was 100.0, with no values falling below 21% or above 100%. 
A histogram and a box plot were generated to visualise the distribution, which revealed a strong skew toward 21% (room air) with only a small number of patients receiving supplemental oxygen at levels such as 40%, 60%, 70%, 80%, 95%, or 100%. 
This pattern is clinically expected in a general emergency triage population.

# Cleaning Steps
The cleaning process began by verifying that all FiO₂ values fell within the physiologically valid range of 21% to 100%. 
No out‑of‑range values were found, so none were removed or set to missing. The 22 missing values were then imputed. The visualisation confirmed that FiO₂ is a discrete clinical parameter, typically delivered via standard oxygen devices that provide specific fractions (e.g., 21%, 40%, 60%, 80%, 100%). Therefore, the mode (the most frequently occurring value) was chosen as the imputation method because it preserves the most common oxygen setting and avoids introducing artificial intermediate values that would not occur in real clinical practice. The mode of the FiO₂ column before imputation was 21.0, and all missing entries were filled with this value.

# Key Findings
No abnormal values were present in the original FiO₂ column, as all measurements were within the 21‑100% range. The distribution was highly skewed toward 21% room air, which is typical for an emergency triage setting where most patients do not require supplemental oxygen. The 22 missing values were successfully imputed with the mode (21%), a choice that maintains clinical plausibility and preserves the real‑world distribution of oxygen settings.
