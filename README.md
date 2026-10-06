# Electoral Threat and Digital Repression

This repository documents my research on how electoral threat shapes incumbents' use of digital repression and how this relationship varies across regime contexts and tactics.

## Research question

When incumbents face electoral threat, how does their use of digital repression change, and which digital tactics do they expand?

## Project overview

I conceptualize **electoral threat** as a pre-election condition that combines meaningful electoral competition with uncertainty about whether the incumbent will retain governing power. The project examines whether this threat changes the overall use of digital repression and whether the relationship varies across levels of electoral democracy.

The empirical analysis uses a country-year panel covering **2000–2020**. Digital repression is measured with multiple indicators capturing filtering, internet and social-media shutdowns, social-media censorship, government and party disinformation, arrests for online political content, and government social-media monitoring.

## Empirical strategy

The project uses several panel-data approaches to evaluate the argument and assess robustness.

- **PanelMatch** for matched panel comparisons around electoral threat
- **Two-way fixed effects (TWFE)** as a benchmark specification
- **FEct and IFEct** as sensitivity analyses
- Event-time and placebo analyses to evaluate timing

## Repository plan

This repository will contain reproducible research materials as they are prepared for public release.

```
.
├── README.md
├── code/
│   ├── 01_data_preparation.R
│   ├── 02_measurement.R
│   ├── 03_panelmatch.R
│   ├── 04_twfe.R
│   ├── 05_fect_ifect.R
│   └── 06_figures_tables.R
├── documentation/
├── figures/
└── tables/
```

Raw data will only be shared where redistribution is permitted. Where source data cannot be redistributed, the repository will document how to obtain the data and reproduce the analysis.

## Research status

An earlier version of this project was presented at the **2026 Summer Conference of the Korean Association of International Studies**, Seoul, June 24, 2026.

## Author

**Jiyun Ko**  
M.A. Candidate in Political Science, Dongguk University

Research interests include state repression, political violence, political competition, regime survival, digital politics, and information control.
