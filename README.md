# hs4002-labrador-2026

The research question that our study aims to answer is:
**How is parental education associated with traditional gender-role attitudes, and do religiosity, attitudes to science and technology, and political culture moderate this association?**

We use the WVS Wave 7 Singapore data (N = 2,012).


Parental education is examined separately using:

Q277R: Mother's education level

Q278R: Father's education level


Both variables are ordinal and contain three ordered categories:

Lower education

Middle education

Higher education


Traditional gender-role attitudes are represented by the composite score constructed in 02_scale_reliability.ipynb (Q28–Q31), where higher scores indicate more traditional attitudes.

The moderators are religiosity (Q164), two science and technology measures and four political culture measures, built in 06_pca.ipynb.

## Research Hypotheses

**H1a:** Mother's education level is associated with traditional gender-role attitudes.

**H1b:** Father's education level is associated with traditional gender-role attitudes.

**H1d:** Religiosity moderates the association between parental education and traditional gender-role attitudes.

**H1e:** Attitudes to science and technology moderate this association.

**H1f:** Political culture moderates this association.

Each H1 has a matching H0 (no association / no moderation). The other notebooks have their own hypotheses (H1c, H1g–H1j), which are written at the top of each one.

All tests are two-tailed because we are looking at whether there is an association, rather than predicting a specific direction beforehand.


## Order to run things
From the raw WVS_Wave_7_Singapore data in the data folder, run the notebooks in the code folder in order, from 01 to 10.

If you re-run 04, run 05 and 06 straight after it, because 04 rebuilds the cleaned dataset and 05 and 06 add their variables back into it.

You will need:

```
pip install pandas numpy scipy statsmodels stargazer scikit-learn prince matplotlib plotnine
```
