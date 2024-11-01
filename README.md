# NBA Player Career Duration Prediction with Naive Bayes

## Introduction
This project builds a Naive Bayes model to predict the career longevity of NBA players, focusing on whether they remain in the league for at least five years. The model uses rookie-year performance data and feature-engineered insights to make predictions.

## Dataset
- **Observations**: 1,341 players
- **Features**: Rookie-year stats and engineered features
- **Target**: Boolean value indicating a career duration of five years or more

## Data Dictionary

The dataset contains performance metrics for 1,341 NBA players. Each feature below represents a different aspect of a player's performance:

| Column Name      | Type | Description                                                                 |
|------------------|------|-----------------------------------------------------------------------------|
| `fg`             | int  | Made field goal percentage                                                  |
| `3p`             | int  | Made 3-point field goal percentage                                          |
| `ft`             | int  | Made free throw percentage                                                  |
| `reb`            | int  | Average rebounds per game                                                   |
| `ast`            | int  | Average assists per game                                                    |
| `stl`            | int  | Average steals per game                                                     |
| `blk`            | int  | Average blocks per game                                                     |
| `tov`            | int  | Average turnovers per game                                                  |
| `target_5yrs`    | int  | Player's career duration over five years (0 = no, 1 = yes)                 |
| `total_points`   | int  | Total points scored across five years                                       |
| `efficiency`     | int  | Total points divided by minutes played per game                             |

> **Note**: A "field goal" in basketball means the ball has gone through the hoop during play, resulting in points scored. Players score 2 or 3 points based on their position from the hoop, and 1 point for free throws due to fouls.

## Objective
Create a model that assists NBA management by identifying players with high long-term potential. This tool can inform decisions on training, scouting, and player retention.

## Model Overview
Naive Bayes is chosen for its ability to handle new, evolving data. By analyzing performance from rookie years, it offers a quick and adaptable approach to predicting player longevity.

## Key Steps
1. **Data Collection**: Extracted NBA player performance records.
2. **Feature Engineering**: Optimized features based on prior analysis.
3. **Model Training**: Implemented Naive Bayes for binary classification on career duration.
4. **Evaluation**: Assessed model accuracy and performance with test data.
