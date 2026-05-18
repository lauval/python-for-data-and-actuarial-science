# Python for Data Science — An Introduction for Actuaries

A hands-on Jupyter notebook designed for actuarial science students transitioning from R to Python. It covers core Python syntax, data manipulation with pandas, visualisation with matplotlib and seaborn, and statistical modelling with statsmodels, all applied to a real-world motor insurance dataset.

## Dataset

The notebook uses the **freMTPL2freq** dataset: ~678,000 French motor third-party liability policies from the [CASdatasets](https://dutangc.github.io/CASdatasets/) R package, hosted on [OpenML](https://www.openml.org/d/41214). It includes claim counts, exposure periods, driver demographics, vehicle characteristics, bonus-malus coefficients, and regional data.

The dataset downloads automatically on first run via `sklearn.datasets.fetch_openml` and is cached locally as a CSV for subsequent runs.

## Getting Started

**Prerequisites:** Python 3.11+

1. Clone this repo:
   ```bash
   git clone <repo-url>
   cd <repo-name>
   ```

2. (Recommended) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate        # macOS/Linux
   venv\Scripts\activate           # Windows
   ```

3. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels scikit-learn jupyter
   ```

4. Launch the notebook:
   ```bash
   jupyter notebook python_for_actuaries.ipynb
   ```

## What's Inside

| Part | Topic | Key Concepts |
|------|-------|-------------|
| 1 | Python Syntax Essentials | Variables, types, collections, control flow, list comprehensions, functions |
| 2 | Data Manipulation (pandas) | Loading CSVs, filtering, groupby, aggregation, column transforms, sorting |
| 3 | Visualisation (matplotlib & seaborn) | Bar charts, histograms, box plots, heatmaps, scatter plots, subplots |
| 4 | Statistical Modelling (statsmodels) | OLS regression, Poisson GLM with exposure offset, risk relativities, diagnostics |

Each part includes exercises with blank cells for you to complete. R equivalents are noted in comments throughout so you can map concepts across.

## Resources

If you get stuck or want to go deeper, these are worth bookmarking.

### Python Fundamentals

- [Python Official Tutorial](https://docs.python.org/3/tutorial/) — the authoritative walkthrough of core language features.
- [Real Python](https://realpython.com/) — well-written tutorials on practically every Python topic, with a search that actually works.

### Pandas

- [pandas Getting Started Tutorials](https://pandas.pydata.org/docs/getting_started/intro_tutorials/) — the official step-by-step guides, organised by task (selecting data, creating plots, reshaping, etc.).
- [pandas API Reference](https://pandas.pydata.org/docs/reference/) — when you know a method exists but can't remember the arguments.
- [Comparison with R](https://pandas.pydata.org/docs/getting_started/comparison/comparison_with_r.html) — an official pandas page that maps R/dplyr operations to their pandas equivalents. Extremely useful for your transition.

### Visualisation

- [Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/index.html) — start with the "Introductory" section.
- [Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html) — covers the logic behind the library and walks through each plot type.
- [Python Graph Gallery](https://www.python-graph-gallery.com/) — visual catalogue of chart types with copy-paste code. Great for "I want something that looks like *this*" moments.

### Statistical Modelling

- [statsmodels Documentation](https://www.statsmodels.org/stable/index.html) — comprehensive, with examples for GLMs, time series, and diagnostics.
- [statsmodels GLM Guide](https://www.statsmodels.org/stable/glm.html) — specific reference for generalised linear models (Poisson, Gamma, Tweedie, etc.).
- [scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html) — for when you move beyond GLMs into machine learning territory.

### Actuarial / Insurance-Specific

- [Actuarial Data Science Tutorials](https://www.actuarialdatascience.org/ADS-Tutorials/) — by the Swiss Association of Actuaries. Several tutorials use this exact freMTPL2 dataset with both R and Python code.
- [CASdatasets Documentation](https://dutangc.github.io/CASdatasets/) — the source R package. Useful for understanding the dataset variables and finding the companion severity dataset (`freMTPL2sev`).
- [French Motor Claims Tutorial (GitHub)](https://github.com/lorentzenchr/Tutorial_freMTPL2) — a Python notebook focused on the same dataset with scikit-learn integration.

### Quick References

- [Python for R Users Cheat Sheet (DataCamp)](https://www.datacamp.com/cheat-sheet/python-for-r-cheat-sheet) — side-by-side syntax comparison.
- [pandas Cheat Sheet (DataCamp)](https://www.datacamp.com/cheat-sheet/pandas-cheat-sheet-for-data-science-in-python) — one-page visual reference for common pandas operations.