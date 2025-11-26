# Multi-Scale Network Analysis of Professional League of Legends
## Hybrid Player–Team Graph Model for Match-Winner Prediction

**[View the published website here.](https://lol-graph-network-analysis.onrender.com)**

### Author: CJ Jones
### Institution: Georgetown University
### Date: Summer 2025

This project develops a hybrid, multi-scale graph learning model to predict winners of professional League of Legends matches by combining both player-level performance and team-level temporal dynamics within a single heterogeneous network. Using data from Oracle’s Elixir covering LCK and LPL matches from 2019–2024, the pipeline constructs a unified graph where each game links team nodes to the five players from their previous match while preserving chronology. Ego-subgraphs centered on each focal match are extracted to ensure strictly historical context, and a custom relational Graph Attention Network is trained to produce win probabilities. Although the model achieves modest accuracy (52.4%) and AUC (0.56)—below the best team-only baseline—it consistently beats random chance and demonstrates that integrating micro-level player form with macro-level team momentum is both feasible and informative. The project establishes a reusable graph construction pipeline and identifies key limitations and architectural opportunities for future improvement in esports prediction models.