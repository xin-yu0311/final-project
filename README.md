# Final Individual Project - ANOVA using YRBS 2007

## Student Information
- Name: 王心妤
- Student ID: T113370209

## Project Repository
(https://github.com/xin-yu0311/final-project/tree/main)

## Presentation Video
[Paste your YouTube video link here]

## Selected Research Question
**The Relationship Between Physical Activity and BMI Percentile Among Students**

Research question:

> Do students who meet the recommended level of physical activity have different BMI percentiles than those who do not?

## Background

Regular physical activity is an important factor for maintaining a healthy body weight. This project investigates whether students who were physically active for at least 60 minutes per day on five or more of the past seven days have different BMI percentiles compared with students who did not meet this physical activity recommendation.

## Variables

### Explanatory Variable (X)
`PhysicalActivity5OrMoreDays`

This variable records the number of days students were physically active for at least 60 minutes during the past seven days. In this project, it is recoded into a two-group variable named `QN80_group`:

- Met recommendation: 5 or more days
- Did not meet recommendation: fewer than 5 days

### Response Variable (Y)
`BMIPCT`

BMI percentile among students.

## Methods Used

Main statistical method:
- One-Way ANOVA

Additional analyses:
- Descriptive statistics
- Group mean comparison
- 95% confidence interval for the difference in group means
- Bar chart of group means
- Boxplot of BMI percentile by group
- Histogram of BMI percentile
- Assumption checking using residual diagnostics

## Key Results

- Analytic sample size: n = 12,894
- Mean BMI percentile, met recommendation: 64.38
- Mean BMI percentile, did not meet recommendation: 65.10
- Difference in means: -0.71
- F statistic: 1.943
- p-value: 0.163
- 95% CI for difference in means: [-1.70, 0.27]

## Final Conclusion

The one-way ANOVA result does not show a statistically significant difference in mean BMI percentile between students who met and did not meet the physical activity recommendation at alpha = 0.05. Students who met the recommendation had a slightly lower mean BMI percentile, but the difference was small and not statistically significant. Because the YRBS data are observational and self-reported, the result should be interpreted as an association, not causation.

## Project Structure

```text
final-project/
  README.md
  data/
    raw/
    processed/
  notebooks/
  outputs/
    figures/
    tables/
    summary/
  report/
  references/
```

## Main Code File

The complete reproducible workflow is in `notebooks/00_full_analysis.ipynb`. This notebook includes data loading, variable recoding, cleaning, descriptive summaries, visualization, one-way ANOVA, assumption checking, saved outputs, and interpretation.
