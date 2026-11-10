# Phase 2 — Exploration Log (Draft)

Data source: monthly branch summary workbook. Branches are anonymized as Branch A–H in source row order. The workbook has 41 monthly columns (April 2023–August 2026). Financial values are shown only as ratios, shares, or indices in these charts.

**Important:** This is a preliminary exploratory analysis of branch-level sales only. It does not establish salesperson performance or customer decline. Figures are not substitutes for client feedback.

## Findings

### Chart 1: Overall monthly sales index

![Chart 1](phase2_charts/01_overall_sales_index.png)

**Observation:** The final month index is 326, compared with 100 in April 2023; part of this increase may reflect additional branches.

### Chart 2: Branch contribution in August 2026

![Chart 2](phase2_charts/02_latest_branch_share.png)

**Observation:** The two largest branches account for 71.7% of August 2026 sales.

### Chart 3: Branch growth over observed operating periods

![Chart 3](phase2_charts/03_branch_period_growth.png)

**Observation:** 6 of 7 branches with at least 12 recorded months grew between their initial and final three-month averages; these windows differ by branch.

### Chart 4: Branch monthly growth heatmap

![Chart 4](phase2_charts/04_growth_heatmap.png)

**Observation:** Growth and contraction vary substantially by branch and month; gray cells represent missing or noncomparable periods.

### Chart 5: Frequency of month-to-month declines

![Chart 5](phase2_charts/05_negative_growth_frequency.png)

**Observation:** Across branches with recorded month-to-month comparisons, the frequency of monthly declines ranges from 0% to 56%.

### Chart 6: How branch share changes over time

![Chart 6](phase2_charts/06_branch_share_over_time.png)

**Observation:** Branch contribution shifts over time; new branches entering the record change the distribution.

### Chart 7: Monthly pattern within each calendar year

![Chart 7](phase2_charts/07_within_year_month_pattern.png)

**Observation:** Different years do not show an immediately identical monthly shape; 2023 and 2026 have incomplete calendar-year coverage.

### Chart 8: Dead end: lifetime totals vs monthly averages

![Chart 8](phase2_charts/08_lifetime_vs_monthly.png)

**Observation:** Lifetime totals and per-month averages use different exposure periods, so lifetime sales alone are not a fair way to compare branches.

## Data audit issues to carry forward

- Monthly sales values include missing cells and non-numeric dashes. These are treated as unobserved months, not zero sales.
- The operating history differs by branch: Branch A: 41 months, Branch B: 41 months, Branch C: 41 months, Branch D: 24 months, Branch E: 41 months, Branch F: 27 months, Branch G: 28 months, Branch H: 3 months.
- The published grand-total row differs from the summed branch values in 14 months (using a tolerance of 0.01); calculate monthly totals from the branch rows before using them.
- The branch summary uses mixed text and Excel-serial dates and includes grand totals and growth rows interleaved with sales rows.
- These charts do not evaluate salesperson performance; the representative-level sheets require separate profiling and reconciliation.

## Working takeaway (hypothesis)

The sales story is not just whether the business is growing overall, but how growth and instability differ across branches; the final visualization should connect this to salesperson performance where data supports it.
