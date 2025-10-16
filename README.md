# Particle Size Analysis Project

## Project Overview

This project involves the statistical analysis of nanoparticle size data obtained from Dynamic Light Scattering (DLS) measurements. The main objective is to explore the relationship between particle size and experimental conditions (primarily temperature), identify any outliers, and perform regression analysis to understand potential influencing factors.

---

## Objectives

- Analyze the distribution of nanoparticle sizes.
- Detect and report outliers in the dataset.
- Perform regression analysis to evaluate the effect of temperature on particle size.
- Summarize key statistical metrics for particle size.

---

## Tools and Libraries Used

- **Python 3.x**
- **Pandas** for data manipulation and summary statistics.
- **NumPy** for numerical operations.
- **Statsmodels** for statistical modeling and regression analysis.
- **Matplotlib / Seaborn** (optional) for data visualization.
- Jupyter Notebook / Google Colab as the interactive coding environment.

---

## Data Description

- **DLS_Particle_Size_nm:** Numeric variable representing the nanoparticle size measured in nanometers.
- **Temperature_C:** Numeric variable representing the temperature at which the measurement was taken.
- Dataset contains 500 observations.

---

## Analysis Performed

### 1. Descriptive Statistics

- Calculated count, mean, standard deviation, minimum, quartiles, and maximum for nanoparticle size.
- Summary:
  - Count: 500
  - Mean particle size: ~150.23 nm
  - Standard deviation: ~24.46 nm
  - Range: 74.09 nm to 249.71 nm

### 2. Outlier Detection

- Used Z-score and Interquartile Range (IQR) methods to detect outliers.
- Identified 3 extreme outliers using Z-score method (threshold ±3).
- Identified 4 outliers using IQR method (1.5 * IQR rule).

### 3. Regression Analysis

- Conducted Ordinary Least Squares (OLS) regression to examine the effect of temperature on particle size.
- Results:
  - Regression coefficient for Temperature: -0.8374 (not statistically significant, p = 0.247)
  - R-squared: 0.003, indicating temperature explains very little variance in particle size.
- Conclusion: No strong evidence that temperature affects particle size in this dataset.

---

## Key Findings and Interpretation

- The particle size measurements are generally consistent with a mean of about 150 nm and moderate variability.
- A small number of extreme values were detected as outliers and may require further investigation or exclusion depending on context.
- Temperature does not appear to significantly influence particle size within the observed range.

---

