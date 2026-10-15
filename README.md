# Estimating UBC Parking Volume and Revenue

An independent analysis estimating parking volume and parking revenue at The University of British Columbia (UBC) Vancouver campus for 2025.

## Overview

How many vehicles park at UBC Vancouver in a year, and how much revenue might that parking generate?

The public information I found did not directly answer these questions. This project uses transportation statistics, published parking rates, and explicit assumptions to develop an estimate.

The analysis is an example of **Fermi estimation**: breaking a question into smaller quantities, using available evidence, and making assumptions where direct measurements are unavailable.

## Results

| Metric | Baseline estimate |
|---|---:|
| Annual parking instances | 3,477,240 |
| Annual parking volume sensitivity range | 3,259,912–3,694,568 |
| Assumed revenue per parking instance | $5 CAD |
| Estimated annual parking revenue | $17,386,200 CAD |
| Estimated revenue sensitivity range | $16,299,562–$18,472,838 CAD |

These are independent, assumption-based estimates, not official UBC statistics or reported financial results.

The annual parking figure represents accumulated daily estimates, not the number of unique vehicles or individual transactions.

## Methodology

The analysis follows four main steps:

1. **Estimate inbound vehicle trips.** The UBC Transportation Status Report reports 46,800 single-occupant vehicle trips to and from campus. Assuming inbound and outbound trips are approximately equal gives an estimated 23,400 inbound trips per day.
2. **Estimate daily parking demand.** Apply an 80% baseline proportion of drivers parking on campus, based on a survey finding referenced in the transportation report.
3. **Account for seasonal differences.** Estimate demand across approximately 126 Winter Session academic weekdays and the remaining 239 days, assuming the latter have 25% of Winter Session demand.
4. **Estimate revenue.** Apply a baseline of $5 per estimated parking instance, given the lack of public information establishing the actual mix of permit holders and short-term parkers.

A sensitivity analysis considers parking proportions of 75%, 80%, and 85%.

## Limitations

The estimates depend on assumptions that could not be fully validated using the public information collected for this project.

Important limitations include:

- The parking proportion is based on a 2022 survey and may not reflect 2025 behaviour.
- The assumed seasonal demand reduction may not accurately represent weekends, holidays, and summer activity.
- The $5 revenue baseline is an assumption, not a measured average.
- The analysis does not fully account for off-campus parking or differences between parking facilities.
- The resulting annual parking estimate should not be interpreted as a count of unique vehicles.

Current transaction records, permit sales, occupancy data, and more detailed seasonal observations would help produce a more reliable estimate.

## Approach and tools

This project was completed as a quantitative analysis using publicly available information and manual calculations.

It was **not** a software-development or dataset-processing project. I did not build a Python pipeline or obtain a transaction-level parking dataset; the available public information was insufficient to calculate the requested figures directly. The analysis instead focuses on how the available evidence can be used to construct a transparent estimate, while documenting the assumptions required.

## Repository contents

- `report/Parking_Analysis.pdf` — the project report.
- `references/sources.md` — source links and references used in the analysis.

## Author

Sameer Shankar

This is an independent project based on publicly available information. It is not affiliated with or endorsed by the University of British Columbia.

