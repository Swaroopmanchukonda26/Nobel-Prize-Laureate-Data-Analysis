# Historical Demographics & Global Distribution Analysis of Nobel Laureates

A comprehensive exploratory data analytics dashboard investigating over a century of human achievement (1901–2020) by parsing structural data trends, geographic research concentrations, and demographic insights across six prize fields using Pandas, Plotly, and Seaborn.

## 🚀 Key Architectural Discoveries
* **The Demographics Shift:** Across the entire historical timeline, female laureates make up a tight 6.2% of all winners. However, granular split bars show higher representations in Peace, Literature, and Medicine compared to severe imbalances in Physics.
* **Geographical Research Layouts:** Interactive hierarchical Sunburst mapping reveals extreme concentration disparities between nations. For example, France's discoveries are entirely centralized inside Paris, whereas Germany's breakthrough systems are highly decentralized across a wide grid of university hubs.
* **The Age of Brilliance:** Local non-linear regression trends (`lowess=True`) prove that hard science laureates (Physics, Chemistry) are receiving their awards significantly later in life (climbing from an average age of 50 up to over 70), while Peace Prize winners display the exact opposite trend, becoming younger over time.

## 🛠️ Data Science Toolkit Used
* **Languages & Platforms:** Python, Google Colab
* **Exploration & Feature Engineering:** Pandas (`.value_counts()`, `pd.to_datetime()`, string split regex fractional parsers, and custom multi-index cumulative sum tracking).
* **Geo-Spatial Plotting:** Plotly Express (`px.choropleth`) tracking three-letter international ISO location code layers.
* **Hierarchical Clusters:** Plotly Express (`px.sunburst`) mapping parent-to-child nested array paths (Country ➔ City ➔ Institution).
* **Advanced Regressions:** Seaborn (`sns.lmplot`) using custom multi-row row category frames and local `lowess` moving average smoothers.
