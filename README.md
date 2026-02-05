# Football Talent Compression
Has elite football experienced talent distribution compressed over time, with a rising floor and a narrowing ceiling?

## Abstract
Over the past decade, elite football has undergone significant tactical, physical, and organizational change. While contemporary players benefit from improved coaching, conditioning, and tactical structure, there is growing debate over whether modern football produces fewer truly dominant individuals than previous eras.

This project investigates whether the English Premier League has experienced talent distribution compression, a phenomenon characterized by a rising baseline standard of performance (the “floor”) alongside reduced or more volatile separation between the league’s most dominant players and the positional average (the “ceiling”).

Using player-season data from the Premier League spanning the 2015–16 to 2023–24 seasons, the analysis measures talent distribution at the individual level across four position groups (forwards, midfielders, defenders, and goalkeepers). Position-specific performance metrics are standardized within each season to estimate ceiling dominance (top individual z-scores) and floor strength (25th-percentile performance among regular players).

Rather than assessing absolute quality, the study focuses on distributional change: how the spread of individual performance within positions has evolved over time. The project is implemented as a reproducible and modular analysis pipeline, designed to generalize to other leagues and competitions in future work.

By reframing player quality as a distribution rather than a ranking, this project provides a framework for understanding why modern football may appear simultaneously more competitive and less individually dominant, even as overall performance standards continue to rise.

## Project Scope

### Current Implementation
- League: English Premier League (EPL)
- Seasons: 2015–16 to 2023–24
- Unit of analysis: Individual player-season
- Positions analyzed: Forwards, Midfielders, Defenders, Goalkeepers
- Focus: Talent distribution dynamics (floor vs ceiling) within positions
- Output:
  - Reproducible analysis pipeline
  - Processed metrics dataset
  - Position-specific visualizations
  - Long-form analytical write-up

### Planned Extensions
- Replication across other top European leagues (La Liga, Serie A, Bundesliga, Ligue 1)
- Expansion to leagues with structural parity mechanisms (e.g., MLS)
- Alternative dominance metrics (e.g., WAR-style composite impact models)


## Pipeline Overview
1. Ingest player-season data by league and season
2. Assign players to standardized position groups
3. Compute role-specific impact metrics
4. Estimate ceiling dominance and floor strength using within-season standardization
5. Aggregate results across seasons
6. Visualize talent distribution trends over time
