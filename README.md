<div align="center">

# GDP Dashboard 🌍

**An interactive web dashboard for exploring and comparing the GDP of countries from 1960 to 2022.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)

</div>

---

## Overview

A small Streamlit app that loads World Bank GDP data and lets you pick countries and a time range, then shows how their economies have grown.

**Why it exists:** it is a hands-on introduction to Streamlit (data loading, caching, interactive widgets, Community Cloud deployment), the framework also used for [SchrödArt](https://github.com/Alyaa203/P2i).

> **Credit:** this app is based on Streamlit's official [GDP dashboard template](https://github.com/streamlit/gdp-dashboard-template).

---

## Features

- **Year range slider** from 1960 to 2022
- **Country picker** (defaults: Germany, France, UK, Brazil, Mexico, Japan)
- **Line chart** of GDP over time, one line per country
- **Summary cards** showing each country's GDP in the final year (in billions of USD) and its growth factor over the selected period
- **Cached data loading** so the app stays fast when you change the filters

---

## Tech stack

| Area | Tools |
| --- | --- |
| Language | Python |
| Data | pandas, [World Bank Open Data](https://data.worldbank.org/) (CSV in `data/`) |
| Web interface and charts | Streamlit |
| Dev environment | Dev Container (GitHub Codespaces) |

---

## Getting started

Requires Python 3.9 or later.

```bash
git clone https://github.com/Alyaa203/gdp-dashboard.git
cd gdp-dashboard
pip install -r requirements.txt
streamlit run streamlit_app.py
```

Then open http://localhost:8501.

You can also open the repo in **GitHub Codespaces**: the Dev Container installs everything and starts the app automatically.

---

Licensed under the Apache 2.0 licence (see [`LICENSE`](LICENSE)).
