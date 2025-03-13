# 2022LoLProAnalysis
*Exploring how Side Selection and Early Game Statistics Affect Professional Match Results*

## Overview
This project analyzes a 2022 League of Legends Esports dataset to explore how side selection and early game statistics affect match outcomes. It aims to uncover trends and insights that can drive strategic decision-making for professional teams.

## Dataset Description
- **Side Selection**: Indicates which side (red or blue) a team plays on.
- **Early Game Statistics**:  
  - Combined metrics: Gold, Experience, and Creep Score at both the 10 and 15 minute marks.
- **Match Outcome**:  
  - **Result**: Encoded as 1 (win) or 0 (loss), where the mean value is directly proportional to the win rate.

## Key Findings and Insights
- **Blue Side Advantage**:  
  - Teams playing on the blue side exhibit a higher overall win rate compared to the red side.
  
- **Statistical Differences**:  
  - At both the 10 and 15 minute marks, blue side teams show a positive mean difference in combined statistics, whereas red side teams show a negative difference.
  - Blue side teams also have a higher KDA (kill-death-assist) ratio compared to red side teams.

- **Correlation with Win Rate**:  
  - Differences in gold, experience, and overall statistics are directly proportional to win rates, indicating that early game performance is a strong predictor of match outcomes.

## Leveraging the Dataset for Decision-Making
In professional League of Legends, especially in best-of formats (best-of-3 or best-of-5), a team that loses a game gains priority in side selection for subsequent games. Given the statistically higher win rate for blue side teams, this analysis suggests that teams can optimize their strategy by:
- Prioritizing blue side selection when given the choice.
- Using early game metrics to predict match outcomes and adjust tactics accordingly.

## Suitable Machine Learning Problem Type
Based on the analysis, a **classification problem** is most appropriate for this dataset:

- **Target Variable**:  
  - The match outcome (win=1, loss=0) makes it a binary classification problem.

- **Rationale**:
  - The goal is to predict the probability of a win based on early game statistics and side selection.
  - Common classification algorithms like logistic regression, decision trees, random forests, or SVM can be applied to model the relationship between the predictors and the match result.
  
- **Application**:
  - A trained classification model can serve as a decision support tool for professional teams, informing them about the potential impact of side selection and early game performance on overall match outcomes.

## Conclusion
This analysis demonstrates that early game metrics and side selection play a crucial role in determining match outcomes in professional League of Legends. By applying classification techniques, teams can leverage historical data to make informed decisions, potentially gaining a competitive edge in tournaments.
