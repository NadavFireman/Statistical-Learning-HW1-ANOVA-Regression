# Statistical Learning - ANOVA & Regression (HW1)

**Home Assignment 1 (Grade 95, M.Sc. Data Science, HIT). Five problems on the analysis of variance and its equivalence to linear regression — one-way and two-way ANOVA, hand-derived OLS/MLE estimators, post-hoc multiple-comparison corrections, and non-parametric alternatives. Every manual derivation is verified against statsmodels.**

## Overview
The assignment works through the general linear model on real datasets — clothing prices, investment-strategy returns and a toxicology experiment on rats. The recurring theme is that ANOVA and regression with dummy variables are two views of the same model: throughout, hand calculations (sums of squares, F-statistics, effect estimates, confidence intervals) are derived from first principles and then confirmed numerically with statsmodels. The work also covers what to do when the classical assumptions fail — diagnostics, multiple-comparison control, and rank-based alternatives.

## Key Features
- **ANOVA ↔ Regression Equivalence:** One-way ANOVA and its dummy-variable regression form derived side by side, showing identical F-statistics and p-values, with the intercept and coefficients interpreted against a reference group.
- **Manual OLS/MLE Derivation:** A no-intercept threshold model estimated from scratch — OLS in both direct and matrix form, shown to coincide with the MLE — plus closed-form expectation and variance, then validated numerically.
- **Two-Way ANOVA:** Additive (no-interaction) two-factor model on the balanced rats dataset, with main-effect F-tests, the parallel regression parametrization, and goodness-of-fit measures.
- **Post-Hoc Multiple Comparisons:** Fisher's LSD, Bonferroni and Benjamini-Hochberg (FDR) corrections compared across every pairwise contrast, with explicit discussion of the family-wise error tradeoff.
- **Assumption Diagnostics:** Residuals-vs-fitted, scale-location, Normal Q-Q and residual histograms, plus Shapiro-Wilk tests — identifying heteroscedasticity and non-normality where present.
- **Non-Parametric Alternatives:** Kruskal-Wallis and Mann-Whitney U (with corrections) as rank-based fallbacks when normality and equal-variance assumptions are violated, cross-checked against the parametric conclusions.
- **Simple Linear Regression:** Full ANOVA table built from summary statistics — sums of squares, F-test, R² and significance — from the raw moments alone.

## Tech Stack
- **Language:** Python
- **Statistics:** statsmodels, SciPy, scikit-posthocs
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn

## Repository Structure
- `Statistical_Learning_HW1.ipynb`: Full solution notebook — all five problems, with derivations, code and analysis.
- `Statistical_Learning_HW1.pdf`: PDF export of the executed notebook.
- `class.exe.01.xlsx`: Clothing-price and investment-strategy datasets (Questions 1 and 3).
- - `rats.csv`: Toxicology experiment dataset — poison × treatment response times (Question 4).
- `Assignment_Instructions_1.pdf`: Original course assignment.
