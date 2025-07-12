# NBA Shot Analysis Suite (2024 Season)

## Overview
This project analyzes over 200,000 shots from the 2024 NBA season to understand what factors most impact the likelihood of a successful field goal. Using machine learning models — including logistic regression, decision trees, and neural networks — we uncover actionable insights to improve player shot selection and coaching strategies.

## Tools Used
- Python (pandas, scikit-learn, matplotlib)
- Jupyter Notebook
- Machine Learning: Logistic Regression, Decision Tree, Neural Network

## Research Questions
1. Does game environment (home/away) or player position impact shot success?
2. Which shot types and zones are most valuable?
3. What features most influence the probability of a made shot?

## Models Built
| Model                  | Description                                        | Accuracy |
|------------------------|----------------------------------------------------|----------|
| Logistic Regression    | Baseline model for interpretability                | 62.1%    |
| Decision Tree depth=5/7| Most interpretable and aligned with project goal   | 62.6%    |
| Neural Network (3,3)   | Slightly higher accuracy but less explainable      | 62.98%   |

Despite similar accuracy, decision trees provided clearer insights into shot selection and feature importance.

## Key Insights
- Shot distance, action type, and zone range were the most predictive features
- 3-point shots from the corners had higher-than-average success rates
- Mid-range shots (8–16 ft) were significantly more successful than very short-range shots outside the restricted area
- Home vs. away status had no significant effect on shot outcomes

## Recommendations
- Prioritize corner 3s, running layups, and jump shots
- Avoid shots inside 8 ft unless they’re in the restricted area
- Practice and encourage attempts from left/right side center zones
- Use player-specific heatmaps to guide training programs

## Extras 
-the player shot success module is still being tweaked to accomodate any analysis on individual players 


## Files Included
- `NBA_Shots_Decisiontree.ipynb` – Decision tree modeling of shot success
- `NBA_shot_distance_by_pos.ipynb` – Shot range analysis by position
- `nba_shots_player_shot_success.ipynb` – Player-specific input tool for shot analysis
- `NBA_shots_neuralnet.ipynb` – Neural network model for predicting shot success
- `NBA shots 'report'.docx` – Full write-up with model results and recommendations
