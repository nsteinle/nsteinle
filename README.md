# Nathan Steinle

Hi! I research theoretical models, data science tools, and machine learning applications in relativistic and multi-messenger astrophysics and beyond! I am a physics and mathematics educator at the undergraduate and graduate level. Below you can find some open-source research and educational materials for physics and data science.

[ORCID](https://orcid.org/0000-0003-0658-402X) · [Website](https://nsastrophysics.github.io)

---

## Research and Software

### classSNRcat

---coming soon!


### [creditdecide](https://github.com/nsteinle/creditdecide)

A Python package that turns a labeled table into a decision rule that can be explained and monitored, shown on 30,000 real credit-card accounts. It includes:

- **Data quality and leakage control** — checks for duplicates and undocumented codes, and a group-aware split so that no duplicate input crosses from the test split into training
- **Decisions** — calibrated probabilities, capacity and cost policies, and a benchmark against the best one-line rule
- **Explanations and uncertainty** — reason codes for every flagged account, and 95% bootstrap intervals for the test results
- **Monitoring and fairness** — population stability reports for new data, and a fairness audit by protected group
- **Data layer and reporting** — DuckDB SQL, tested against pandas, and tables for a [Tableau Public dashboard](https://public.tableau.com/app/profile/nathan.steinle/viz/creditdecidewhichcreditcardaccountstoreview/creditdecide)

On the bundled data, reviewing the riskiest 10% of accounts reaches 31.5% of next month's defaulters, and the best one-line rule does as well at the same volume.

[PyPI](https://pypi.org/project/creditdecide/) · [Zenodo](https://doi.org/10.5281/zenodo.24059025) · [Dashboard](https://public.tableau.com/app/profile/nathan.steinle/viz/creditdecidewhichcreditcardaccountstoreview/creditdecide) · MIT license

### [declinecast](https://github.com/nsteinle/declinecast)

A Python package that forecasts how much oil a well will produce in its first three years from its first months of production, with low and high cases that are checked against what the wells went on to produce. It is shown on 8,344 horizontal wells in Colorado's DJ Basin, from the state regulator's public production records. It includes:

- **Data layer and data quality** — a DuckDB SQL panel built from 9.4 million regulator records, tested against pandas, that counts every defect, from records filed twice to a change of file format
- **Bayesian inference** — a neural posterior estimator, trained once on 500,000 simulated wells, that returns each well's posterior Arps decline parameters, noise and downtime in a fraction of a second
- **Validation** — simulation-based calibration and coverage checks on simulated wells, and a test set of wells first produced in 2020 and later, locked before any scoring and scored once
- **Forecasts and flags** — P90, P50 and P10 cumulative oil to 36 and 60 months, and a flag for wells unlike the ones the model was trained on
- **Benchmarks and uncertainty** — least-squares Arps, a history multiplier, a type curve and per-well MCMC, compared with bootstrap intervals over whole operators, and tables for a [Tableau Public dashboard](https://public.tableau.com/app/profile/nathan.steinle/viz/declinecast36-monthcumulativeoilforecastswithrangesforDJBasinwells/declinecast)

On 1,463 test wells forecast from 12 months of production, the 80% range contains the 36-month outcome for 81% of wells, against 48% for least-squares Arps. A simple history multiplier does as well, and per-well MCMC on the same model is as accurate but takes 2.5 to 9 times more compute per forecast.

[PyPI](https://pypi.org/project/declinecast/) · [Zenodo](https://doi.org/10.5281/zenodo.24095678) · [Dashboard](https://public.tableau.com/app/profile/nathan.steinle/viz/declinecast36-monthcumulativeoilforecastswithrangesforDJBasinwells/declinecast) · MIT license


---

## Teaching

### [Introductory Physics, Math, and Chemistry](https://github.com/nsteinle/intro-physics-math-chemistry-teaching)

Lecture notes and problem-solving resources developed and used with high school students in Texas. Topics include:

- AP Physics — oscillations, waves, circuits, and Ohm's law
- AP Chemistry — phase diagrams
- Geometry — ratios and proportions

### [Astrophysics and Machine Learning](https://github.com/nsteinle/astrophysics-machine-learning-teaching)

Lecture notes, lesson plans, and runnable Jupyter coding modules developed and used at the University of Manitoba and the University of Winnipeg. Topics include:

- **Gravitational-wave astrophysics** — graduate lecture notes covering GW theory, detection, and multi-messenger observations (Fall 2023, U Manitoba)
- **Machine learning for astronomy** — undergraduate lecture notes on ML/AI, plus a Python coding module using LIGO data for GW signal classification (Fall 2025, U Manitoba)
- **Pulsar timing arrays** — graduate lecture notes on PTA science and radio astronomy, plus a data analysis module using public NANOGrav 15-yr data (Spring 2026, U Manitoba)
- **Gravitational waves from supernovae** — undergraduate lesson plan and coding worksheet (2024–2025, U Manitoba)
- **WITP 2024** — gravitational-wave astrophysics lecture worksheets (Summer 2024, U Winnipeg)

All teaching materials are licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Instructor versions are available on reasonable request.

---

## Contact

📫 nsastrophysics@gmail.com



<!---
nsteinle/nsteinle is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
