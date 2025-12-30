# Unicorn Growth Strategy – SQL Project

SQL case study on global unicorn companies, using DataCamp’s database as a starting point and extending it into a **portfolio-grade analysis** with a **growth, strategy, and investor-oriented lens**.

This project focuses on understanding **where value is created in the private tech ecosystem**, how fast companies scale, and how capital efficiency and industry dynamics differ across sectors and geographies.

---

## Motivation

This project was built to move beyond intuition and analyze the startup and venture ecosystem through **structured, data-driven reasoning**.

Rather than treating unicorn data as a purely exploratory exercise, the goal was to approach it from a **growth and capital allocation perspective**: understanding **which industries consistently create value, how quickly companies scale, and where capital is most efficiently deployed**.

Given a long-term interest in strategy, growth, and investment-driven roles, this project serves both as a **technical SQL showcase** and as a framework to reason more rigorously about how high-growth businesses are built, funded, and scaled.

---

## Context and Goals

* Identify **industries and geographies** that concentrate unicorn creation and aggregate valuation.
* Understand **market phases** (early growth, expansion, boom, normalization) in the global unicorn ecosystem.
* Evaluate **capital efficiency**, valuation dispersion, and time-to-scale across sectors.
* Practice **analyst-style SQL** (CTEs, window functions, composite metrics) with a clear **business and investment mindset**, not just descriptive EDA.

---

## Dataset

* **Source**: DataCamp Unicorn Companies PostgreSQL database
* **Scope**:

  * Private companies valued above $1B
  * Global coverage across multiple industries
* **Key fields**:

  * Company, industry, country, city
  * Year founded, year achieving unicorn status
  * Valuation, total funding raised, investors

---

## What Is Analyzed

### 1. Trend Analysis & Market Dynamics

* Unicorn creation by **year and industry**
* Industry share of yearly unicorn creation
* **Year-over-year growth** by sector
* Identification of structural vs cyclical growth patterns

### 2. Valuation & Unit Economics

* Average vs median valuations by year and industry
* Valuation skewness and distribution analysis
* Valuation bands (1–2B, 2–5B, 5–10B, 10B+)
* Industry-level “private market cap” concentration

### 3. Market Concentration & Competition

* Industry ranking by total market capitalization
* Market share and **Herfindahl-Hirschman Index (HHI)** contributions
* Identification of fragmented vs concentrated sectors

### 4. Cohort & Velocity Analysis

* Time to reach unicorn status (founding → unicorn year)
* Fastest and slowest scaling industries
* Differences in scaling velocity across sectors

### 5. Geographic & Funding Patterns

* Unicorn density by **country and city**
* Regional valuation hubs and industry specialization
* Capital efficiency: valuation vs total funding raised
* Identification of high-multiple vs capital-intensive sectors

### 6. Advanced Predictive Indicators

* **Industry Momentum Score (0–100)** combining:

  * Recency of unicorn creation
  * Total market capitalization
  * Average valuation levels
* Strategic prioritization of industries based on forward-looking momentum

---

## Key Insights (Executive Summary)

* A small set of industries concentrates the majority of unicorn creation and valuation, with **Fintech, Internet Software & Services, AI, and E-commerce** leading structurally.
* **2021 represents a clear outlier boom**, followed by normalization rather than collapse.
* Significant differences exist between:

  * **Volume-driven industries** (many unicorns, lower average valuations)
  * **Value-concentrated industries** (fewer companies, higher capital intensity)
* Capital efficiency and time-to-scale vary meaningfully by sector, implying **different risk-return profiles** for investors and corporate acquirers.

---

## Tech Stack

* **Language**: SQL (PostgreSQL)
* **Core concepts**:

  * CTEs
  * Window functions (LAG, RANK, rolling calculations)
  * Conditional aggregations
  * Percentiles and distribution analysis
  * Composite scoring models
* **Environment**: PostgreSQL database hosted on DataCamp

---

## Repository Structure

```
sql/
│── trend_analysis.sql
│── valuation_analysis.sql
│── market_concentration.sql
│── cohort_velocity.sql
│── geographic_patterns.sql
│── momentum_score.sql

notebooks/
│── exploration_notes.md
│── intermediate_checks.sql

outputs/
│── result_tables.csv
│── selected_visuals/
```

---

## Who This Is For

* Data Analysts and aspiring **Growth / Strategy professionals** looking to see SQL applied to real business decisions.
* Candidates targeting **VC, Corporate Development, or M&A-adjacent roles**.
* Anyone interested in translating raw startup data into **actionable strategic insights**.

---

## Next Steps

* Incorporate macro-economic cohorts to contextualize unicorn creation cycles.
* Extend the dataset with funding rounds and exits to link **valuation to realized returns**.
* Build lightweight visualizations or dashboards on top of the SQL outputs.
