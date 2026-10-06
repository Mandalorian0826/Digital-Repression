# Electoral Threat and Digital Repression

This repository documents my research on how electoral threat shapes incumbents' use of digital repression and how that response varies across levels of democracy.

## Research question

Do incumbents use more digital repression when they face an electoral threat, and is the effect largest at intermediate levels of democracy?

## Argument

I define **electoral threat** as the risk that incumbents will lose governing power through an election that satisfies two conditions.

1. **Minimal competition** means that incumbent defeat is institutionally possible because opposition participation is permitted, multiple parties are legal, and voters have a choice among candidates.
2. **Outcome uncertainty** means that incumbents cannot confidently expect to retain governing power in the approaching election.

The argument focuses on the period before voting, when opposition campaigning and mobilization can still affect electoral outcomes. Digital repression can help incumbents restrict opposition communication, disrupt coordination, obtain information through surveillance, and support more targeted intervention.

The project evaluates two expectations.

- **H1:** Incumbents facing electoral threat use higher levels of digital repression than incumbents not facing electoral threat.
- **H2:** The marginal effect of electoral threat on digital repression is largest at intermediate levels of democracy and smaller at lower and higher levels.

## Data and measurement

The study uses a **country-year panel covering 179 countries from 2000 through 2020**, with 3,741 observations before estimator-specific restrictions.

The primary outcome is Feldstein's **eight-item Digital Repression Index (DRI)**. It combines:

- internet filtering
- internet shutdowns
- social-media shutdowns
- social-media censorship
- government disinformation
- party/candidate disinformation
- arrests for online political content
- government social-media monitoring

The moderator is V-Dem's **Electoral Democracy Index**, measured in the preceding year.

## Empirical strategy

The analysis uses two complementary panel-data approaches.

### PanelMatch

PanelMatch estimates the effect of entering the electoral-threat condition among treatment onsets. The primary design:

- compares treated onsets with untreated country-years in the same calendar year
- requires the same treatment history over the previous three years
- refines matched sets using Mahalanobis distance
- uses lagged pretreatment covariates and the lagged outcome
- retains up to five matched controls
- estimates effects from the threat year through three subsequent years
- evaluates pretreatment comparability with placebo contrasts
- uses 1,000 country-cluster bootstrap replications

An election-restricted specification further limits controls to country-years that also precede a classifiable but nonthreatening election.

For H2, treated onsets are grouped using the lagged four-category electoral-democracy classification, and synchronized bootstrap draws are used to compare intermediate and extreme regime categories.

### Two-way fixed effects

TWFE models complement the PanelMatch estimates by evaluating heterogeneity across the continuous Electoral Democracy Index.

The nonlinear specification interacts electoral threat with:

- the lagged Electoral Democracy Index
- its squared term

Models include country and year fixed effects, the lagged moderator and its square, and the remaining lagged adjustment variables. Inference uses **Driscoll-Kraay standard errors** to address cross-sectional and serial dependence.

## Repository plan

Reproducible materials will be organized as they are prepared for public release.

```
.
├── README.md
├── code/
│   ├── 01_data_preparation.R
│   ├── 02_construct_electoral_threat.R
│   ├── 03_construct_dri.R
│   ├── 04_panelmatch.R
│   ├── 05_twfe.R
│   ├── 06_diagnostics.R
│   └── 07_figures_tables.R
├── documentation/
├── figures/
└── tables/
```

Raw data will only be shared where redistribution is permitted. Where source data cannot be redistributed, the repository will document how to obtain the original data and reproduce the analysis.

## Research status

An earlier version of this project was presented at the **2026 Summer Conference of the Korean Association of International Studies**, Seoul, June 24, 2026.

## Author

**Jiyun Ko**  
M.A. Candidate in Political Science, Dongguk University

Research interests include state repression, political violence, political competition, regime survival, digital politics, and information control.
