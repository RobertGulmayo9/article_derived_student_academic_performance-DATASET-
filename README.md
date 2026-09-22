[README.md](https://github.com/user-attachments/files/32519931/README.md)
# Article-Derived Student Academic Performance Dataset

Source: Rolly T. Dagdagui (2022), "Predicting Students’ Academic Performance Using Regression Analysis."

## Important limitation

This is an **article-derived dataset**, not the original 596-student raw dataset.

The article describes a 596-student dataset and reports group-level tables, correlations, and the final regression coefficients, but it does not publish the individual student records. Therefore, this repository must not be presented as the original student-level dataset.

## Files

- `article_derived_dataset.csv` — combined long-form table for easy Colab import
- `academic_performance_summary.csv` — published performance summaries by sex, course, strand, and type of school
- `predictor_correlations.csv` — published predictor correlation coefficients and p-values
- `regression_coefficients.csv` — published regression equation coefficients
- `study_metadata.csv` — study/model metadata

## Colab import

```python
import pandas as pd

url = "https://github.com/RobertGulmayo9/article_derived_student_academic_performance-DATASET-/blob/main/dataset/article_derived_dataset.csv"
df = pd.read_csv(url)
df.head()
```

## Reproducibility note

The article reports an adjusted R² of 67.3% and the regression equation:

Y = 37.088 + 0.406(GW) + 0.399(GA) + 0.935(S) - 0.241(C)

These published model results should be treated as reported results from the article, not as results independently reproduced from raw student-level observations.
