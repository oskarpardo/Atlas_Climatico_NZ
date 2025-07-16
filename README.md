# 📈 New Zealand Agro-Climatic Adaptation Atlas for 2050

![Python](https://img.shields.io/badge/python-3.x-blue.svg) ![Pandas](https://img.shields.io/badge/pandas-2.x-blue.svg) ![NumPy](https://img.shields.io/badge/numpy-1.2x-blue.svg) ![Streamlit](https://img.shields.io/badge/streamlit-1.x-orange.svg) ![Plotly](https://img.shields.io/badge/plotly-5.x-orange.svg) ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

**A full-cycle data analysis project to assess climate risk and model adaptation strategies for New Zealand's key primary industries.**

---

### ➡️ [View Live Interactive Dashboard](link-to-be-added)

*A GIF of the final, interactive dashboard will be embedded here for immediate visual demonstration.*

---

## 1. Project Vision & Value Proposition

This project simulates a high-level strategic consulting engagement, designed to go beyond conventional data analysis. The objective is to build a prototype **Climate Risk Assessment Tool**. The value proposition is to demonstrate the ability to transform disparate, complex data into an interactive tool that facilitates long-term strategic decision-making. The final output not only presents findings but also offers a solution that a stakeholder, such as a viticulturist or a government planner, can use to explore scenarios and plan for adaptation.

## 2. The Business Problem

New Zealand's primary industries are the backbone of its export economy and a core part of its national identity. However, they face a tangible and growing threat from climate change. This project addresses the following specific and measurable risks:

* **Viticulture:** Global warming is causing "harvest compression," accelerating grape ripening, which impacts quality and creates logistical bottlenecks during the harvest season.
* **Kiwifruit:** Rising winter temperatures threaten "loss of winter chill." Kiwifruit varieties like Hayward require a minimum number of hours at low temperatures to ensure uniform bud break and an abundant harvest. This puts the viability of the crop at risk in key regions like the Bay of Plenty.
* **Dairy:** The increase in "heat stress days" (temperatures > 25°C) can reduce cattle feed intake, decrease milk production, and affect the overall health of the animals.

## 3. Research Hypotheses

To address this problem, the analysis will be guided by the following testable hypotheses:

* **H1 (Viticulture):** An increase in average temperatures and extreme heat days in key regions like Marlborough and Hawke's Bay will positively correlate with harvest compression and greater year-over-year variability in grape production.
* **H2 (Dairy):** The projected increase in "heat stress days" in primary dairy regions like Waikato and Canterbury will negatively correlate with milk production per cow.
* **H3 (Kiwifruit):** The projected decrease in "winter chill units" in the Bay of Plenty will negatively correlate with the yield of green kiwifruit (Hayward) varieties.

---

## 4. Tech Stack

* **Language:** Python
* **Analysis & Manipulation:** Pandas, NumPy, GeoPandas
* **Database:** SQLite (via SQLAlchemy)
* **Visualization:** Plotly, Matplotlib, Seaborn
* **Interactive Dashboard:** Streamlit
* **Version Control:** Git & GitHub
* **Virtual Environment:** venv / conda

---

## 5. Repository Structure

The project is logically organized to facilitate navigation, maintenance, and reproducibility.

```
/
├── data/
│   ├── raw/          # Original, unprocessed data files
│   └── processed/    # Cleaned database and intermediate files
├── notebooks/        # Jupyter Notebooks for exploration and analysis
├── src/              # Python scripts with reusable functions
├── app/              # Code for the Streamlit application
├── .gitignore
├── requirements.txt  # List of dependencies for reproducibility
└── README.md         # This file, the project's central document
```
---

## 6. Data Sources

Data acquisition was proactively planned to integrate information from multiple government agencies, a key challenge of the project.

| Dataset                  | Source                            | Key Variables                                  | Format/Access                   | Relevance to Hypothesis                                                  |
| :----------------------- | :-------------------------------- | :----------------------------------------------- | :------------------------------ | :----------------------------------------------------------------------- |
| **Historical Climate** | NIWA DataHub                      | Daily Max/Min Temp, Precipitation              | CSV (requires registration)     | Baseline for calculating historical metrics like `heat_stress_days` and `winter_chill_units`. |
| **Climate Projections** | NIWA / MfE Portal                 | Temp, Rainfall, Heat Days >25°C under SSP scenarios | NetCDF or CSV                   | Core of the future risk analysis.                                        |
| **Agricultural Production**| Stats NZ (Aotearoa Data Explorer) | Hectares planted, total production by region | CSV (via ADE) or Excel          | Key dependent variable for correlation and regression models.            |
| **Regional Boundaries** | Stats NZ / LINZ                   | Polygon geometries of regional councils        | Shapefile or GeoJSON            | Essential for geospatial visualization and data aggregation.             |

---

## 7. Methodology & Project Phases

*This section will be filled out as the project progresses, summarizing the key steps in each phase.*
* **Phase 1: Planning & Design:** Definition of objectives, hypotheses, and the data acquisition plan.
* **Phase 2: Data Acquisition & Engineering:** ETL process (Extract, Transform, Load), cleaning, joining, and feature engineering.
* **Phase 3: Exploratory Analysis & Modeling:** Visualization, correlation analysis, and scenario modeling.
* **Phase 4: Communication & Deployment:** Building and deploying the interactive dashboard with Streamlit.

---

## 8. Key Findings & Conclusions

*This section will be filled out at the end of the project with the most important discoveries and the answers to the research hypotheses.*

---

## 9. Installation & Usage

*This section will explain how someone else can clone the repository, install the dependencies with `pip install -r requirements.txt`, and run the analysis and application.*

---

## 10. License

This project is licensed under the MIT License.
