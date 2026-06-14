# FIFA World Cup 2026 Quarter-Final Qualification Analysis

A Power BI analytics project that evaluates the quarter-final qualification potential of teams participating in the 2026 FIFA World Cup by comparing their pre-tournament performance with historical FIFA World Cup quarter-finalists (1954–2022).

## Project Objective

The goal of this project is to identify teams whose current form most closely resembles that of historical World Cup quarter-finalists and rank them using a custom-built **Quarter-Final Qualification Score**.

## Dataset

### Historical Dataset (1954–2022)

The historical dataset consists of FIFA World Cup quarter-finalists and includes:

* Matches Won, Drawn, and Lost (last 20 matches before the World Cup)
* Win Percentage
* Goals For (GF)
* Goals Against (GA)
* Goal Difference (GD)
* GF/Match
* GA/Match
* GD/Match
* FIFA Ranking

> Note: The 1974, 1978, and 1982 World Cups were excluded due to the absence of a quarter-final stage in those tournament formats.

### 2026 World Cup Participants

A separate dataset was created for all teams participating in the 2026 FIFA World Cup using the same performance metrics.

---

## Methodology

### 1. Historical Benchmarking

Historical quarter-finalists were analyzed to establish benchmark values for:

* Win Percentage
* GF/Match
* GA/Match
* GD/Match
* FIFA Ranking

### 2. Team Style Classification

Historical teams were categorized into:

* Attacking Powerhouse
* Defensive Specialist
* Balanced Contender
* Vulnerable Side
* Mixed Profile

based on their attacking and defensive performance metrics.

### 3. Z-Score Normalization

To compare metrics measured on different scales, Z-score normalization was applied.

Formula:

```text
Z = (X - μ) / σ
```

Where:

* X = Current team value
* μ = Historical average
* σ = Historical standard deviation

Positive Z-scores indicate above-average performance compared to historical quarter-finalists.

### 4. Composite Strength Index (CSI)

A weighted combination of standardized metrics was used to calculate a Composite Strength Index representing a team's current form.

Metrics included:

* Win %
* GF/Match
* GA/Match
* GD/Match
* FIFA Ranking

### 5. Historical Pedigree Score

A Historical Pedigree Score was created using:

* Previous FIFA World Cup Quarter-Final Appearances

This metric captures long-term tournament consistency.

### 6. Quarter-Final Qualification Score

The final score combines:

* Current Form (CSI)
* Historical Pedigree

to rank teams according to their quarter-final qualification potential.

---

## Dashboard Features

* Historical Quarter-Final Analysis
* Team Style Distribution
* Performance Trend Analysis
* Composite Strength Index Ranking
* Historical Pedigree Analysis
* Quarter-Final Qualification Score Ranking
* Interactive Power BI Visualizations

---

## Tech Stack

* Power BI
* DAX
* Microsoft Excel

---

## Key Skills Demonstrated

* Data Collection & Cleaning
* Data Modeling
* DAX Calculations
* Statistical Analysis
* Z-Score Normalization
* Data Visualization
* Dashboard Development
* Sports Analytics

---

## Future Enhancements

* Integration of Expected Goals (xG)
* Player-level performance metrics
* Machine Learning-based prediction models
* Semi-final and winner prediction models

---

## Author

**Nishant Karn**

Electronics and Instrumentation Engineering Student | Power BI Developer | Sports Analytics Enthusiast
