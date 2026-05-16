# Canadian Cheese & Climate Analysis

An exploratory data analysis project looking at whether a province's climate is related to the kind of cheese it produces.

---

## Project Overview

This notebook was completed as part of the Canadian Cheese Foundation Data Analyst Intern assessment. I combined two public datasets — the Canadian Cheese Directory and historical Canadian weather data — to explore whether temperature patterns across provinces have any relationship with cheese production volume or cheese characteristics like moisture and fat content.

---

## Datasets

| Dataset | Source | Description |
|---|---|---|
| `cheese_data.csv` | [Kaggle — Canadian Cheese Directory](https://www.kaggle.com/datasets/noahjanes/canadian-cheese-directory/data) | 1,042 Canadian cheeses with attributes including moisture %, fat level, milk type, and province |
| `Canada_Temperature_Data.csv` | [Kaggle — Canada Weather](https://www.kaggle.com/datasets/hemil26/canada-weather) | Monthly temperature records from weather stations across Canada (1917–2017) |

---

## What's in the Notebook

- **Data cleaning** — handles missing values in both datasets, drops rows missing key analytical columns, fills descriptive nulls
- **Climate profile** — builds annual, winter, and summer average temperatures per province using 2000–2017 weather data as a contemporary baseline
- **Cheese summary** — aggregates moisture %, fat level, and cheese count by province
- **Merged analysis** — joins both datasets on province code for cross-dataset comparison
- **Two visualizations** — see below
- **Discussion** — written summary of findings and inferences

---

## Visualizations

**Visualization 1 — Climate vs. Cheese Production**

Two scatter plots: annual average temperature vs. cheese count (with province labels and trend line), and winter average temperature vs. average cheese moisture content.

**Visualization 2 — Cheese Characteristics by Province**

Two horizontal bar charts showing average moisture % and proportion of higher-fat cheeses by province, ordered coldest to warmest so climate patterns are easy to spot.

---

## Key Findings

- **Production volume** doesn't follow temperature. Quebec produces the most cheeses by far despite being one of the colder provinces — cultural history and dairy industry size matter more than climate.
- **Winter temperature and moisture** show a moderate positive correlation (r = +0.41). Provinces with harsher winters tend to produce higher-moisture cheeses (soft, washed-rind styles), possibly because cool, humid cellars favour those ageing conditions.
- **Fat level** varies by province but doesn't map cleanly to temperature — BC has the highest proportion of higher-fat cheeses, which likely reflects its local artisan market more than its climate.

---

## Tools Used

- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook
