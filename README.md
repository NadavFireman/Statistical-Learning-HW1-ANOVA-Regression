# Statistical Learning - ANOVA & Regression (HW1)

**Home Assignment 1 (Grade 95, M.Sc. Data Science, HIT). Five problems on ANOVA and its equivalence to linear regression — every manual derivation verified against statsmodels.**

## Overview
The general linear model, worked by hand on real datasets — clothing prices, investment returns and a rat-toxicology experiment: derivations from first principles confirmed numerically, plus diagnostics, multiple-comparison control and rank-based alternatives for when the classical assumptions fail.

## Key Features
- **ANOVA ↔ Regression Equivalence:** One-way and two-way (additive, on the balanced rats dataset) ANOVA derived side by side with their dummy-variable regression forms — identical F-statistics and p-values.
- **Manual OLS/MLE Derivation:** A no-intercept threshold model estimated from scratch — OLS in direct and matrix form, coinciding with the MLE — then validated numerically.
- **Post-Hoc Corrections:** Fisher's LSD, Bonferroni and Benjamini-Hochberg (FDR) compared across every pairwise contrast.
- **Diagnostics & Non-Parametric Fallbacks:** Residual plots, Normal Q-Q and Shapiro-Wilk expose heteroscedasticity and non-normality; Kruskal-Wallis and Mann-Whitney U cross-check the parametric conclusions.
- **ANOVA Table from Raw Moments:** Sums of squares, F-test and R² built from summary statistics alone.

## Repository Structure
- `Statistical_Learning_HW1.ipynb`: Full solution notebook — all five problems.
- `Statistical_Learning_HW1.pdf`: PDF export of the executed notebook.
- `class.exe.01.xlsx` / `rats.csv`: Datasets (Q1, Q3, Q4).
- `Assignment_Instructions_1.pdf`: Original course assignment.

---
*Course: Statistical Learning, M.Sc. Data Science, HIT · Python, Pandas, NumPy, statsmodels, SciPy, Matplotlib, Seaborn*
