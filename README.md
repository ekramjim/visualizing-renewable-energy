# Visualizing Renewable Energy

An interactive data visualisation dashboard exploring global renewable energy trends, built with Vega-Lite and hosted on GitHub Pages.

**Live Demo:** [ekramjim.github.io/visualizing-renewable-energy](https://ekramjim.github.io/visualizing-renewable-energy/)

## Overview

This project visualises global renewable energy consumption data sourced from the World Bank. It presents five complementary chart idioms to uncover geographic, temporal, and compositional patterns in renewable energy adoption across countries and regions.

## Visualisations

| Idiom | Chart Type | Description |
|-------|-----------|-------------|
| 1 | Choropleth Map | Global renewable energy share by country |
| 2 | Bar Chart | Country-level renewable energy comparison |
| 3 | Stacked Area Chart | Temporal trends across energy sources |
| 4 | Donut Chart | Compositional breakdown by energy type |
| 5 | Additional Idiom | Supplementary trend analysis |

## Tech Stack

- **Vega** & **Vega-Lite** — declarative grammar for interactive charts
- **Vega-Embed** — embedding and rendering visualisations in HTML
- **Pure.css** — lightweight responsive layout
- **TopoJSON** — geographic boundary data for the choropleth map
- **Python** — data cleaning and preprocessing script
- **HTML/CSS** — dashboard layout and styling

## Data Sources

- [World Bank — Renewable Energy Consumption (% of total final energy consumption)](https://data.worldbank.org/indicator/EG.FEC.RNEW.ZS)
- Natural Earth 110m admin boundaries ()

## Project Structure

```
visualizing-renewable-energy/
├── index.html                        # Main dashboard page
├── data_cleaning_script.py           # Data preprocessing
├── data/
│   ├── complete_renewable_energy_dataset.csv
│   ├── API_EG_FEC_RNEW_ZS_DS2_en_csv_v2_1722.csv
│   ├── ne_110m.topojson              # World map boundaries
│   └── ne_110m_admin_0_countries/
└── Js/
    ├── mapidiom1.vg.json             # Choropleth map spec
    ├── barchartidiom2.vg.json        # Bar chart spec
    ├── stackedAreaChartIdiom3.vg.json
    ├── donutchartIdiom4.vg.json
    └── idiom5.vg.json
```

## Getting Started

No build step required. Open locally or serve via any static file server:

```bash
git clone https://github.com/ekramjim/visualizing-renewable-energy.git
cd visualizing-renewable-energy
# Open index.html in your browser, or:
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## License

MIT
