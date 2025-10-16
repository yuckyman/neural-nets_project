# neural-nets_project

## reference
[this](https://medium.com/@androidmatheny/using-git-and-github-on-group-projects-d636be2cdd4d) link may help if you're unfamiliar with git. 

assuming you have `git` installed, you can just run the following in your terminal and it will download the project folder:
```
git clone https://github.com/yuckyman/neural-nets_project
cd neural-nets_project
```

## cookie cats — phase 1 EDA

This repo includes a notebook that performs basic EDA on the Cookie Cats A/B dataset and produces D1/D7 retention visuals.

### data
- Place the raw CSV at `data/cookie_cats/raw.csv`, or set Kaggle credentials and the notebook will attempt to download automatically:
```
export KAGGLE_USERNAME=your_username
export KAGGLE_KEY=your_key
```

### run the notebook
- Open `notebooks/cookie_cats_eda.ipynb` and run all cells.

### outputs
- Figures: `reports/figures/`
  - `cookiecats_overall_d1_d7.png`
  - `cookiecats_uplift_by_version.png`
  - `cookiecats_retention_vs_gamerounds.png`
- EDA summary: `reports/cookie_cats_eda.md` (links/embed to figures)
- Cleaned table: `data/cookie_cats/clean.parquet`

### what it shows
- Overall D1/D7 retention rates
- Retention uplift by gate version (`gate_30` vs `gate_40`)
- Retention vs early engagement (`sum_gamerounds` deciles)