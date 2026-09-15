# T20 World Cup Power BI Dashboard - Copilot Instructions

## Project Purpose

This project is an interactive Power BI dashboard for analyzing T20 World Cup cricket data from 2014 to 2026.

The current dashboard focuses on:
- Tournament analysis
- Match analysis
- Team analysis
- Batting analysis
- Bowling analysis

Player Analysis is planned but has not been completed yet.

## Technologies

- Microsoft Power BI
- DAX
- Power Query
- Data Modeling
- Data Visualization
- Python for data preparation

## Current Dashboard Pages

1. Home
2. Tournament Overview
3. Match Analysis
4. Team Analysis
5. Batting Analysis
6. Bowling Analysis

### Planned Page

7. Player Analysis

Player Analysis is currently under development and should not be treated as an already completed dashboard page.

## Main Tables

Important tables in the Power BI model include:

- matches
- full_deliveries
- batting_summary
- new_bowling_summary
- Teams
- Teams_Team1
- Teams_Team2
- Teams_Winner
- Players

## Important Columns

### matches

- MatchID
- Date
- Team1
- Team2
- Venue
- City
- TossWinner
- TossDecision
- PlayerOfMatch
- Year
- Tournament
- Toss Impact
- Winner
- Toss Result

### full_deliveries

- MatchID
- BattingTeam
- Batter
- Bowler
- BatterRuns
- TotalRuns
- Wicket
- WicketKind

### batting_summary

- Balls
- Batter
- Boundary Runs
- Fours
- Runs
- Sixes
- StrikeRate

### new_bowling_summary

- Balls
- Bowled
- Bowler
- Caught
- CaughtAndBowled
- Economy
- HitWicket
- LBW
- Overs
- RunOut
- RunsConceded
- Stumped
- TotalDotBalls
- TotalWickets

### Players

- Player

The Players table currently contains player names and is intended for future Player Analysis functionality.

## Current Dashboard Analysis

### Tournament Overview

Current analysis includes:

- Total Matches
- Total Teams
- Total Runs
- Total Wickets
- Total Sixes
- Total Fours
- Matches by Venue
- Matches by Year
- Toss Decision distribution
- Matches by City

### Match Analysis

Current analysis includes:

- Total Matches
- Average Match Score
- Highest Score
- Lowest Score
- Average Wickets per Match
- Matches Won by Toss Winner
- Matches by Toss Winner
- Toss Impact on Match Result
- Average Score by Year
- Average Score by Toss Decision

### Team Analysis

Current analysis includes:

- Matches Played
- Matches Won
- Win Rate
- Total Runs
- Total Wickets
- Average Score
- Team Runs by Year
- Win vs Loss
- Top 10 Teams by Match Wins
- Dynamic team selection

### Batting Analysis

Current analysis includes:

- Total Runs
- Average Runs
- Highest Score
- Total Fours
- Total Sixes
- Average Strike Rate
- Top 10 Batters by Boundary Runs
- Top 10 Six Hitters
- Top 10 Four Hitters

### Bowling Analysis

Current analysis includes:

- Total Wickets
- Total Runs Conceded
- Average Wickets
- Average Economy
- Total Dot Balls
- Total Balls
- Top 10 Wicket Takers
- Top 10 Most Economical Bowlers
- Wickets by Dismissal Type
- Wickets by Year

## DAX Guidelines

When creating DAX:

1. Use the actual table and column names listed above.
2. Do not invent column names.
3. Respect the current filter context.
4. Use SELECTEDVALUE when a calculation depends on a selected team or player.
5. Use TREATAS when a disconnected table needs to filter another table.
6. Use DIVIDE instead of direct division when division by zero is possible.
7. Prefer readable DAX with meaningful measure names.
8. Explain the purpose of a measure before suggesting complex DAX.
9. Check the existing data model before creating calculations that depend on relationships.

## Dashboard Design

The dashboard uses a dark navy and pink theme.

Main colors:

- Page background: #080B2B
- Panel/KPI background: #18213F
- Menu background: #343D5A
- Selected menu: #596681
- Accent pink: #FF1493
- Trend line cyan: #00BFFF
- Border: #3A4568
- Main text: #FFFFFF
- Secondary text: #D0D4E4

Keep visual recommendations consistent with this theme.

## Visualization Guidelines

Prefer:

- KPI cards for important metrics
- Horizontal bar charts for rankings
- Column charts for comparisons
- Line charts for yearly trends
- Donut charts for simple proportions
- Slicers for interactive filtering

Charts should be clean, readable, and consistent with the dashboard theme.

Rounded rectangle panels can be used behind charts with:
- Fill: #18213F
- Border: #3A4568
- Rounded corners
- Minimal or no shadow

## Important Project Rules

When helping with this project:

1. Work with the existing Power BI data model.
2. Use actual table and column names.
3. Do not invent missing data.
4. Do not assume Player Analysis is already completed.
5. If a required column, relationship, image URL, or player information is unavailable, clearly state that.
6. Preserve the existing dashboard's dark navy and pink design.
7. Keep DAX simple, readable, and appropriate for Power BI.
8. When suggesting a new visual, explain exactly which fields should be placed in the Axis, Values, Legend, and Filters.
9. When troubleshooting, first check the table names, column names, data types, relationships, and filter context.

## Project Status

Completed:
- Home
- Tournament Overview
- Match Analysis
- Team Analysis
- Batting Analysis
- Bowling Analysis

In Progress:
- Player Analysis

Future Player Analysis may include:
- Player selection slicer
- Player profile information
- Player runs
- Player wickets
- Fours and sixes
- Strike rate
- Economy
- Other player-level statistics

These Player Analysis features are planned and should be implemented only after verifying that the required player data and relationships are available.
