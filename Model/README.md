## Player Evaluation & Forecasting Model

### Overview
This project is a customizable player evaluation and forecasting model designed to translate underlying performance metrics into long-term projections. The model integrates statistical analysis with baseball-specific context to support objective, data-informed decision-making in player development and roster construction.

A central principle of this model is that player value in baseball is inherently subjective. As a result, the system is built to be flexible, allowing users to define and weight the metrics that best align with their evaluation priorities.

### Objectives
- Provide a flexible framework for evaluating player value based on user-defined criteria
- Model year-to-year player development using historical performance trends
- Identify comparable players to inform expected outcomes
- Generate multi-year projections reflecting both skill progression and variability

Methodology
1. Custom Player Valuation
   - Users select relevant performance metrics (excluding outcome-based metrics such as WAR or wRC+)
   - Custom weights are applied to construct a composite player value score
   - This allows evaluation frameworks to be tailored to different development philosophies or roster needs
2. Recency-Weighted Performance
   - Multi-season data is incorporated with greater emphasis on recent performance
   - Establishes a more accurate representation of current player skill
3. Aging Curve Modeling
   - Historical year-to-year changes in performance are calculated across player populations
   - Age-based trends are applied to estimate future development trajectories
4. Comparable Player Analysis
   - A nearest-neighbor approach is used to identify historically similar players
   - Comparisons are constrained by age and performance profile
   - Expected outcomes are informed by the trajectories of comparable players
5. Multi-Year Forecasting
   - The model iteratively projects player performance across future seasons
   - Outputs reflect both projected skill changes and variability across comparable outcomes

Data
- Historical dataset spanning 10 MLB seasons (2016–2025)
- Includes 1,378 qualified hitter seasons (minimum plate appearance threshold)
- Structured at the player-season level, allowing for longitudinal analysis of performance trends

Outputs
- Composite player value scores based on customizable inputs
- Multi-year projections of player performance
- Comparable player groupings
- Visualizations of projected trends and development trajectories

Tools & Technologies
- Python (primary language)
- Data analysis libraries (pandas, numpy)
- Notebook environment (Jupyter/Google Colab)

Purpose & Application
This model reflects an interest in bridging statistical analysis with on-field understanding of the game. By integrating customizable valuation, aging trends, and comparable player outcomes, it provides a structured yet flexible approach to evaluating and projecting player performance.

Future Improvements
- Incorporate park factors to better isolate the impact of ballparks on in-game events and underlying performance metrics
- Expand the model to include defensive and positional value components
- Integrate pitch-level and batted ball-level data for greater granularity
- Refine similarity metrics for improved comparable player identification
- Develop a more modular pipeline for broader application and scalability

Author
Colton Laurence
Data Science Graduate | Player Development & Baseball Analytics
