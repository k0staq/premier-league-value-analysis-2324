📊 Football Performance & Value Analysis
Premier League 2023/24 — Moneyball-Style Project
🔍 Project Overview

This project applies a Moneyball-style analytical approach to the Premier League 2023/24 season.
The focus is on evaluating attacking performance relative to market value, rather than raw output alone.

The analysis aims to:

identify undervalued attacking players

compare club-level efficiency

highlight young talents and breakout candidates

assess market mispricing using per-90 metrics

The final output is an interactive Power BI report, designed to be both analytically sound and interview-ready.

🎯 Key Analytical Questions

Which forwards deliver above-average attacking output at a reasonable market price?

Which clubs convert squad value into output most efficiently?

Which young players show early signs of breakout performance?

Which players are currently over- or under-performing relative to expected goals?

🧱 Data Sources

FBref — attacking statistics (goals, xG, xAG, minutes)

Transfermarkt — market values and player metadata

Match-level data — supplementary context

Final analytical dataset:

players_value_model_2324_v2.csv

🧠 Feature Engineering & Metrics
Per-90 Normalization

All attacking metrics are calculated per 90 minutes to:

control for playing time

allow fair comparisons across players

Attacking Output Index

A composite metric combining scoring and creativity:

Output Index =
0.6 × Goals (normalized)
+ 0.3 × xG (normalized)
+ 0.4 × xAG (normalized)

Value Metrics

Value Index = Output Index / Market Value

Cost per Output = Market Value / Output Index

Log-adjusted value metrics used to reduce superstar price distortion

🏷 Market Price Tiers

Players are grouped into pricing tiers:

LOW: ≤ €10M

MID: €10M – €60M

ELITE: > €60M

Used consistently across visuals for market segmentation.

📈 Power BI Report Structure
PAGE 1 — Best Value Forwards

This chart highlights forwards who consistently deliver above-average attacking output while remaining undervalued by the market.

Output Index vs Market Value

Bubble size reflects minutes played

Reference lines show league averages

Designed as the main “Moneyball” view

PAGE 2 — League Rankings (Context)

Baseline performance rankings:

Goals per 90

Expected Goals per 90

Expected Assists per 90

Market Value

Provides context, not interpretation.

PAGE 3 — Young Value Stars (U23)

This view isolates under-23 forwards to identify high-upside talents delivering strong output before reaching peak market valuation.

Focuses on:

upside potential

early productivity

market underpricing

PAGE 4 — Over vs Under-Performing Forwards

Comparison of:

Goals per 90 vs Expected Goals per 90

Used to identify:

short-term finishing overperformance

potential regression candidates

Filtered to players with sufficient minutes to ensure reliability.

PAGE 5 — Breakout Candidates (U21)

Targets very young forwards who already combine:

meaningful playing time

tangible attacking output

Designed as a scouting-oriented view rather than long-term projection.

PAGE 6 — Club Efficiency Analysis

Club-level evaluation based on:

average attacking output

cost per unit of output

efficiency relative to league average

Clubs are classified as:

Efficient

Average

Inefficient

This page focuses on organizational efficiency, not star power.

🎨 Design Principles

Dark, analytics-first theme

Minimalist visuals

Consistent color logic

Emphasis on interpretability over complexity

🧠 Key Analytical Choices

Market value used instead of transfer fees (forward-looking expectation)

Per-90 metrics over totals

Log scaling to mitigate elite player value skew

Separate player-level and club-level modeling to avoid aggregation bias

🚀 Outputs

Power BI report (.pbix)

Clean analytical dataset (.csv)

Report screenshots

This README with methodology and insights

📌 Disclaimer

This analysis reflects current-season attacking efficiency and does not represent long-term transfer ROI or tactical fit.

🏁 Final Note

This project was designed to mirror real-world recruitment and performance analysis logic, not just visualize statistics.
