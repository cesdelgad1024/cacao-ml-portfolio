# Flavors of Cacao — Machine Learning Portfolio

End-to-end **machine learning** on the *Flavors of Cacao* dataset (global chocolate
ratings), in Python: sourcing and cleaning the data, then **supervised regression**,
**unsupervised clustering**, **time-series analysis**, and **geospatial
visualization** — finished with an interactive Tableau story.

## Notebooks

| Notebook | Focus |
|---|---|
| [`1_sourcing_open_data.ipynb`](./1_sourcing_open_data.ipynb) | Source, load, and clean the ratings dataset |
| [`2_geo_visualizations.ipynb`](./2_geo_visualizations.ipynb) | **Geospatial visualization** — `folium` choropleth of ratings by region |
| [`3_supervised_machine_learning_regression.ipynb`](./3_supervised_machine_learning_regression.ipynb) | **Supervised regression** — scikit-learn `LinearRegression` on a train/test split, scored with MSE and R² — cocoa percentage alone explains none of the variance in ratings (R² = 0.00) |
| [`4_unsupervised_machine_learning_clustering.ipynb`](./4_unsupervised_machine_learning_clustering.ipynb) | **Unsupervised clustering** — `KMeans` segmentation with the elbow method |
| [`5_sourcing_and_analyzing_time_series.ipynb`](./5_sourcing_and_analyzing_time_series.ipynb) | **Time-series analysis** — `statsmodels` seasonal decomposition, Augmented Dickey-Fuller, and ACF over review dates |

## Stack
`Python` · `pandas` · `numpy` · `scikit-learn` (regression + KMeans) ·
`statsmodels` (time series) · `folium` (geo) · `matplotlib` / `seaborn` · **Tableau**

An interactive [Tableau story](https://public.tableau.com/app/profile/cesar.delgado5456/viz/6_7_flavors_of_cacao/Story1?publish=yes)
presents the headline findings — top manufacturers, cocoa-percentage trends, and the ratings distribution.

## Run it
```bash
git clone https://github.com/cesdelgad1024/cacao-ml-portfolio.git
cd cacao-ml-portfolio
pip install pandas numpy scikit-learn statsmodels folium matplotlib seaborn jupyterlab
jupyter lab   # open the notebooks 1 → 5
```

---
*Part of my path from data analytics into applied ML and cloud AI — see also
**[Verity](https://github.com/cesdelgad1024/verity)**, a fully local agentic RAG
system with an independent-judge evaluation harness.*
