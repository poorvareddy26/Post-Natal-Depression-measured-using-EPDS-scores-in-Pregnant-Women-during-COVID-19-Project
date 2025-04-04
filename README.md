 Analyzing the Impact of Demographic Factors on Postnatal Depression during COVID-19
🧠 Overview
This project investigates the correlation between demographic factors (maternal age, household income, maternal education) and postnatal depression levels in pregnant women during the COVID-19 pandemic, as measured by the Edinburgh Postnatal Depression Scale (EPDS). Using a publicly available dataset from the Pregnancy During the COVID-19 Pandemic (PdP) project on Kaggle, we explore how pandemic-related stressors have disproportionately impacted mental health across different socio-economic groups.

The goal is to identify vulnerable populations and inform better-targeted mental health interventions for pregnant women, particularly during public health crises.

🔍 Research Question
Is there a statistically significant relationship between demographic factors and postnatal depression levels in pregnant women during the COVID-19 pandemic?

Null Hypothesis (H₀): No correlation exists between age, income, education, and EPDS scores.

Alternative Hypothesis (H₁): There is a correlation between these demographic factors and EPDS scores.

📂 Dataset
Source: Kaggle Dataset

Size: 10,772 rows × 16 columns

Key Variables:

Maternal Age (continuous)

Household Income (ordinal categorical)

Maternal Education Level (ordinal categorical)

EPDS Scores (numeric and categorized)

NICU Stay, Mode of Delivery, PROMIS Anxiety Score (not used in final model due to incomplete data)

🧹 Data Cleaning & Preprocessing
Handled missing/null values using median imputation for numeric columns and random sampling for categorical ones.

Outliers in age column were treated using Interquartile Range (IQR) method.

Age was binned into 5 categories for categorical analysis.

EPDS scores were recategorized:

0–6: None/Minimal

7–13: Mild

14–19: Moderate

20–30: Severe

📊 Visualizations
Bar graphs and pie charts for:

Maternal Education

Household Income

Depression Levels

Scatter plot to study Maternal Age vs. EPDS scores.

Segmented bar charts for categorical cross-tabulations.

Heatmap for correlation matrix of variables.

🧪 Statistical Analyses
✅ Normality Checks
Conducted via histograms and Kolmogorov-Smirnov Test.

Maternal Age and EPDS scores were found to be approximately normally distributed.

✅ Chi-Square & Fisher's Exact Tests
Tested association between demographic variables and EPDS categories.

All tests showed significant associations (p < 0.05), rejecting the null hypothesis.

✅ Simple Linear Regression
Between Maternal Age and EPDS Scores:

Strong statistical significance (p < 2.2e-16)

Low R² value (~0.0074) indicates that age alone is not a strong predictor.

✅ Spearman’s Rank Correlation
Negative correlations observed:

Age vs. EPDS: -0.068

Income vs. EPDS: -0.155

Education vs. EPDS: -0.143

✅ Ordinal Logistic Regression
Used to model categorized EPDS scores based on age, income, and education.

Identified moderate predictive power with confidence intervals and residual analysis.

🧠 Key Findings
Maternal Age, Income, and Education levels are significantly associated with postnatal depression levels.

Higher income and education levels were correlated with lower depression scores.

Younger mothers tended to have higher depression scores.

Insights from this research highlight the need for targeted mental health support during crises like pandemics.

Limitations
Could not analyze NICU stay or delivery mode due to missing data.

Correlation ≠ Causation — No temporal causality proven.

R² values were low in simple regression, suggesting other unmeasured factors influence depression scores.

Fisher’s Exact Test has limitations with large datasets.
