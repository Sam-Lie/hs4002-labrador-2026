# hs4002-labrador-2026

The research question that our study aims to answer is:
**How are parental education levels associated with traditional gender-role attitudes?**


Parental education is examined separately using:

Q277R: Mother's education level

Q278R: Father's education level


Both variables are ordinal and contain three ordered categories:

Lower education

Middle education

Higher education


Traditional gender-role attitudes are represented by the composite score constructed in 02_scale_reliability.ipynb, where higher scores indicate more traditional attitudes.

## Research Hypotheses
Our study has two sets of hypotheses.

**Mother's Education**

**H0a:** Mother's education level is not associated with traditional gender-role attitudes.

**H1a:** Mother's education level is associated with traditional gender-role attitudes.

**Father's Education**

**H0b:** Father's education level is not associated with traditional gender-role attitudes.

**H1b:** Father's education level is associated with traditional gender-role attitudes.

All statistical tests we will be conducting will be two-tailed because our hypotheses are looking at whether there is an association between the variables, rather than predicting a specific direction beforehand.


## Order to run things
Run the notebooks in `code/` in numerical order, starting from the raw `WVS_Wave_7_Singapore_Csv_v5.1.csv` in `data/raw/`:

| Notebook | Purpose | Output dataset |
|---|---|---|
| `01_clean.ipynb` | **Initial** cleaning for Presentation 1 (superseded by 04) | `WVS_Singapore_cleaned.csv` |
| `02_scale_reliability.ipynb` | Reverse-coding and Cronbach's alpha for Q28–Q31 | `WVS_Singapore_scored.csv` |
| `03_correlations.ipynb` | Spearman correlations (Presentation 1) | – |
| `04_reclean_full.ipynb` | **Expanded / final cleaning for all later analyses** | `WVS_Singapore_full_cleaned.csv` |
| `05_mother_more_educated.ipynb` | Parental education gap variables | adds to `WVS_Singapore_full_cleaned.csv` |
| `06_pca.ipynb` | PCA and political culture sub-indices | adds to `WVS_Singapore_full_cleaned.csv` |
| `07`–`10` | Moderation, multivariate models, sex differences, item-level logits (10 is exploratory) | – |

**`WVS_Singapore_full_cleaned.csv` (created by notebook 04 and extended by 05 and 06) is the authoritative processed dataset** for notebooks 05–10. Notebooks 01–03 and their datasets are kept so that the Presentation 1 results can be reproduced. Notebook 04 confirms that the variables they share are identical.
