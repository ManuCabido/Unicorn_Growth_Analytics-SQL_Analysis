# Unicorn-Growth-Analytics---SQL-Case-Study
## Unicorn Growth Strategy – SQL Project

SQL case study on global **unicorn companies**, using DataCamp’s database as a starting point but pushing the analysis much further with a growth, strategy and investor‑oriented lens.

***

## Context and goals

- Identify which industries and geographies concentrate new unicorns and where the most attractive growth and investment opportunities may lie.  
- Practice “analyst‑style” SQL (CTEs, window functions, composite metrics) with an M&A / corporate finance perspective rather than only descriptive EDA.

***

## Dataset

- Source: DataCamp unicorn companies PostgreSQL database, with company name, industry, country, founding year, year of unicorn status, valuation and key investors.
- Scope: private companies valued above 1B USD worldwide, across multiple industries (Fintech, Internet Software & Services, E‑commerce, AI, etc.).

***

## What is analyzed

- Dynamics of unicorn creation by year, region and industry, identifying market phases (gradual growth, strong expansion, exceptional boom, normalization).
- Industry “momentum” metrics: number of new unicorns, year‑over‑year growth and share of total valuation to prioritize strategically attractive sectors.
- Valuation structure: mean vs median valuations, valuation bands (1–2B, 2–5B, 5–10B, 10B+) and value concentration by industry to see where private “market cap” accumulates.
- Capital efficiency: relationship between valuation and total funding raised, comparing which industries generate more value per dollar invested.
- Time to unicorn: difference between founding year and unicorn year, segmented by industry and region.

***

## Tech stack

- **Language**: SQL (PostgreSQL).  
- **Key concepts**: CTEs, window functions (ROW_NUMBER, LAG, moving averages), conditional aggregations, case statements to create market phases and valuation bands.
- Environment: PostgreSQL server with the database hosted on DataCamp’s infrastructure.

***

## Repository structure

- `sql/` – core queries, grouped by analysis block (unicorn creation, industry momentum, valuations, capital efficiency, time to unicorn).  
- `notebooks/`  – additional exploration, query testing and interpretation notes.  
- `outputs/` – exported result tables (CSV) and, where relevant, screenshots of the visualizations used in the analysis.

***

## Key insights (executive summary)

- A small set of industries concentrates most new unicorn creation and aggregate valuation, with Fintech and Internet Software & Services standing out in recent years.
- Clear differences appear between “volume” industries (many lower‑ticket unicorns) and “mega‑unicorn” industries where a few companies hold most of the value.
- Average time to reach unicorn status and capital efficiency vary significantly by sector, suggesting different risk‑return profiles for investors and corporates.

***

## Who this is for

- Data Analysts and aspiring **Analytics / Strategy** professionals who want to see SQL applied to a real‑world case with strong business storytelling.  
- People interested in venture capital, M&A and corporate development looking for a quantitative framework to think about high‑growth industries.

***

## Next steps

- Add risk‑oriented metrics (e.g., time to unicorn by macro cohort) and compare them with liquidity cycles.  
- Connect this base with other sources (funding rounds, exits) to extend the analysis from valuations to realized returns.
