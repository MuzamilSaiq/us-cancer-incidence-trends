# U.S. Cancer Incidence Trends (1999–2022)

This project analyzes trends in cancer incidence in the United States from 1999 to 2022 using publicly available CDC/NCI cancer registry data. The analysis examines both age-adjusted incidence rates (risk) and total diagnosed case counts (burden), with stratification by ethnicity, race, and state.

## Executive Dashboard (Power BI Summary)

An executive-facing dashboard version of this analysis is included to provide a high-level, stakeholder-oriented summary of key findings.

The dashboard visualizes:

- National cancer case burden trends (1999–2022)
- Age-adjusted incidence rates by ethnicity (raw and smoothed)
- Age-adjusted incidence trends by race

The dashboard is designed to complement the full analytical notebook by translating statistical results into concise, decision-ready visuals.

**Dashboard export available as PDF.**

## Key Findings
- **Total cancer case burden increased** from approximately 1.3 million to over 1.8 million annual diagnoses, driven by population growth and aging.
- **Age-adjusted incidence rates declined overall**, indicating reduced per-capita cancer risk despite rising case counts.
- **Hispanic populations consistently exhibit lower age-adjusted incidence rates**, consistent with prior literature on the Hispanic health paradox.
- **Racial trends are heterogeneous**: Black and White populations show statistically significant declines, while Asian or Pacific Islander populations contribute minimally to overall temporal trend dynamics.
- **State-level trends vary substantially**, with some states exhibiting steep declines and others flat or increasing trajectories.

## Methods
- Cleaning and preprocessing of state × race × ethnicity × year incidence records
- Aggregation of national annual cancer case counts
- Analysis of age-adjusted incidence rates by ethnicity and race
- Linear regression with race × time interaction terms
- State-level trend estimation via separate regressions

## Notes and Limitations
- Some analyses rely on unweighted means rather than population-weighted rates.
- Analyses focus on temporal trend characterization rather than causal inference.
- COVID-era diagnostic disruptions are visible around 2020.

## Data Source
Cancer incidence data were obtained via **CDC WONDER**, drawing from the *United States and Puerto Rico Cancer Statistics* public-use database maintained by the **Centers for Disease Control and Prevention (CDC)** and the **National Cancer Institute (NCI)**, covering the years 1999–2022.

## References
Ruiz JM, Steffen P, Smith TB. *Hispanic Mortality Paradox: A Systematic Review and Meta-Analysis*.  
**American Journal of Public Health**. 2013;103(3):e52–e60.  
PMID: 23327255.  
https://pmc.ncbi.nlm.nih.gov/articles/PMC3673509/
