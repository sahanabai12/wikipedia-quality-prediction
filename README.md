# Predicting Wikipedia Article Quality from Structural and Content Features

MSc dissertation project (MATH5872M, University of Leeds) — predicting Wikipedia
article quality tiers from six cheap to compute structural features and testing
whether the relationship holds consistently across topic categories.

## Contents
- `Wikipedia_data_collection.ipynb` — parses the Wikipedia XML dumps, extracts the
  six structural features and topic categories and queries the Wikipedia API for
  quality labels via Talk pages.
- `Wikipedia_analysis_final.ipynb` — trains and evaluates Random Forest, XGBoost
  and Logistic Regression on the resulting dataset; reproduces every table and
  figure reported in the dissertation.
- `wikipedia_final.csv` — the final cleaned dataset (1,187 labelled articles).

## Setup
1. Download the 4 dump chunks (`enwiki-latest-pages-articles-multistream1-4`)
   from [dumps.wikimedia.org](https://dumps.wikimedia.org) and place them
   alongside `Wikipedia_data_collection.ipynb`.
2. Install dependencies: `pandas`, `numpy`, `scikit-learn`, `xgboost`,
   `mwxml`, `mwparserfromhell`, `matplotlib`, `statsmodels`.
3. Run `Wikipedia_data_collection.ipynb` to produce `wikipedia_final.csv`
   (or use the version already included in this repo).
4. Run `Wikipedia_analysis_final.ipynb` to reproduce all results.

## Author
Sahana Bai Sankarrao — MSc Data Science and Analytics, University of Leeds
