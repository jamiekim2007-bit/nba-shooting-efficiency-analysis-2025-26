# nba-shooting-efficiency-analysis-2025-26
NBA Shooting Efficiency Analysis
Summary:
This project analyzes the relationship between scoring volume, shooting efficiency, and player position in the NBA using Python and statistical analysis. The goal here is to figure out if players who score more points are more efficient shooters and whether shooting efficiency differs across positions.

Research Questions:
1. Is there a linear relationship between points per game and effective field goal percentage?
2. Do high scoring players (20+ points per game) differ in shooting efficiency from lower-scoring players?
3. Does average shooting efficiency differ across NBA player positions?

Tools utilized:
Python - data
Pandas - cleaning, filtering, and aggeregation
Matplotlib - visualization
SciPy - correlation, regression, hypothesis
Statsmodels - Tukey HSD post-hoc comparisons
Google Colab - environment

Methods:
Filter NBA player statistics for the selected season and players with at least 50 games played.
Ranked high scoring players by effective field goal pct.
Used linear regression and correlation to examine the relationship between ppg and eFG%
Conducted a two sample t-test to compare higher and lower scorers.
Apply ANOVA and Tukey HSD to compare shooting efficiency across 5 posiitons.
Calculated eta-squared to estimate proportion of observed variation associated with position groups.

Key Ideas
Scoring volume & efficiency: PPG showed essentially no linear relationship with eFG% in the sample (correlation = 0.00113).
Higher vs lower scorers: The difference in the average eFG% wasn't statistically significant in the two sample t-test (p=0.1415).
Differences by position: A one-way ANOVA found statistically significant differences in mean eFG% across positions (F=21.6508, p<0.001).
Post-hoc comparisons: Tukey HSD found that centers and significantly higher mean eFG% than each of the other four positions.
Effect size: eta-squared was .247, meaning that around 24.7% o the observed variation in eFG% was associated with differences between position groups in this sample.

Dataset:
Source: NBA,ABA, and BAA statistics dataset on Kaggle
This analysis uses player per game statistics, including points per game, effective field goal percentage, games played, team, and position. Dataset metadata and season coverage should be verified before treating the results as definitive real-world NBA findings due to the season being in the 2025-26 season.

Limitations
The analysis identifies associations and does not establish causation.
Effective fg% doesn't capture every aspect of offensive production such as free throws or playmaking.
Player position alone doesn't account for shot selection, playing style, or individual roles.

Improvements in the Future:
Investigate 3pt shooting and shot selection.
Compare positions using additional statistical tests and confidence intervals
Explore multiple seasons to see if these patterns persist over time.
Develop an interactive dashboard for exploring player statistics

This project was created as a personal sports analytics and statistical analysis portfolio project
