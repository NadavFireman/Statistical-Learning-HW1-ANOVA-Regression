# Statistical Learning - ANOVA & Regression (HW1)

**Home Assignment 1 (Grade 95, M.Sc. Data Science, HIT). Five problems on the analysis of variance and its equivalence to linear regression — every manual derivation verified against statsmodels.**

## Overview
The assignment works the general linear model on real datasets — clothing prices, investment returns and a rat-toxicology experiment — deriving the calculations (sums of squares, F-statistics, effect estimates, confidence intervals) from first principles and confirming them numerically. It also covers what to do when classical assumptions fail: diagnostics, multiple-comparison control, and rank-based alternatives.

## Key Features
- **ANOVA ↔ Regression Equivalence:** One-way ANOVA and its dummy-variable regression form derived side by side — identical F-statistics and p-values, coefficients interpreted against a reference group.
- **Manual OLS/MLE Derivation:** A no-intercept threshold model estimated from scratch — OLS in direct and matrix form, shown to coincide with the MLE — then validated numerically.
- **Two-Way ANOVA:** Additive two-factor model on the balanced rats dataset, with main-effect F-tests and the parallel regression parametrization.
- **Post-Hoc Corrections:** Fisher's LSD, Bonferroni and Benjamini-Hochberg (FDR) compared across every pairwise contrast.
- **Diagnostics & Non-Parametric Fallbacks:** Residual plots, Normal Q-Q and Shapiro-Wilk tests expose heteroscedasticity and non-normality; Kruskal-Wallis and Mann-Whitney U cross-check the parametric conclusions.
- **ANOVA Table from Raw Moments:** A full simple-regression ANOVA table — sums of squares, F-test, R² — built from summary statistics alone.

## Repository Structure
- `Statistical_Learning_HW1.ipynb`: Full solution notebook — all five problems.
- `Statistical_Learning_HW1.pdf`: PDF export of the executed notebook.
- `class.exe.01.xlsx`: Clothing-price and investment datasets (Q1, Q3).
- `rats.csv`: Toxicology dataset — poison × treatment response times (Q4).
- `Assignment_Instructions_1.pdf`: Original course assignment.

---
*Course: Statistical Learning, M.Sc. Data Science, HIT · Python, Pandas, NumPy, statsmodels, SciPy, Matplotlib, Seaborn*
