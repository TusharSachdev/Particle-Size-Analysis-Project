# Particle Size Analysis Project

## Project Overview

This project focuses on analyzing the **Dynamic Light Scattering (DLS) Particle Size** data for different materials under varying conditions, primarily temperature. The objective is to understand how factors like temperature and material type influence the particle size distribution and whether these factors significantly affect the particle size.

---

## Objectives

- To assess the distribution and variability of particle size measured by DLS.
- To evaluate the effect of **Temperature** on particle size using linear regression.
- To investigate whether different **Materials** result in significantly different particle sizes using ANOVA.
- To identify and analyze outliers in the particle size data.
- To explore potential interaction effects between Temperature and Material.
- To ensure statistical assumptions are met for valid inference.

---

## Tools and Libraries Used

- **Python**: Main programming language used for data analysis.
- **Pandas**: Data manipulation and cleaning.
- **NumPy**: Numerical operations.
- **Statsmodels**: Statistical modeling including OLS regression and ANOVA.
- **Matplotlib / Seaborn** (optional): Visualization of data distributions and relationships.

---

## Data Description

- **Data Source**: Experimental DLS particle size measurements for various samples.
- **Key Variables**:
  - `DLS_Particle_Size_nm`: Particle size measured in nanometers.
  - `Temperature_C`: Temperature in degrees Celsius during measurement.
  - `Material`: Type of material/sample.
  - `Sample_ID`: Unique identifier for each sample.

- **Data Summary** (example):
  - Number of observations: 500
  - Particle size mean: ~150 nm
  - Particle size range: ~74 nm to ~250 nm
  - Presence of some outliers identified by z-score and IQR methods.

---

## Analysis Performed

### 1. Exploratory Data Analysis (EDA)
- Summary statistics for particle size.
- Visualization to inspect data distribution and identify outliers.

### 2. Outlier Detection
- Calculated z-scores and Interquartile Range (IQR) to detect outliers.
- Identified and flagged outliers for further consideration.

### 3. Regression Analysis
- Performed **Ordinary Least Squares (OLS)** regression to test the relationship between particle size (`DLS_Particle_Size_nm`) and temperature (`Temperature_C`).
- Result: Temperature was **not a significant predictor** of particle size (p > 0.05).

### 4. Analysis of Variance (ANOVA)
- Tested for differences in particle size across different material groups.
- Ensured there were multiple materials in the dataset to perform valid ANOVA.
- Interpreted results for group differences.

### 5. Interaction Effects
- Investigated if interaction between temperature and material influences particle size.

### 6. Assumption Checks
- Checked normality of residuals.
- Tested homoscedasticity and linearity assumptions.

---

## Key Findings and Interpretation

- **Temperature** does not significantly affect particle size within the observed range.
- Particle size varies among different **Materials**; however, statistical significance depends on having multiple groups.
- Some samples were identified as outliers, which may influence the analysis.
- No strong evidence of interaction effects between temperature and material.
- Overall, particle size is relatively stable across tested conditions but varies by material type.

---

