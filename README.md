# PUBG Game Winner Prediction

🧩 1. Project Overview

This project focuses on predicting the win probability of a player in the popular battle-royale game PUBG.
The goal is to:

Analyze player performance statistics.

Understand which gameplay factors (kills, damage, distance, etc.) most influence winning.

Build a predictive LSTM model that estimates a player’s probability of winning based on match data.

This project demonstrates the integration of data analysis, deep learning, and model interpretation to gain insights into in-game dynamics and player strategies.

🧠 2. Model Summary

| **Model Used**                               | **Description**                                                                                                                                                    | **Performance Summary**                                                                                                 |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| **LSTM (Long Short-Term Memory)**            | Deep learning model designed to capture sequential patterns in player match data. It learns temporal dependencies (how early-game actions affect final placement). | Achieved a **Mean Absolute Error (MAE)** of ~0.045 and strong alignment between predicted and actual win probabilities. |

The LSTM model outperformed traditional regressors in understanding time-based patterns, making it ideal for predicting evolving gameplay outcomes.

🧾 3. Dataset Used

Dataset Source: PUBG Finish Placement Prediction – Kaggle


Key Features:

-kills	

-damageDealt	

-walkDistance, rideDistance, swimDistance	

-boosts

-weaponsAcquired

-headshotKills

-killStreaks

-numGroups	

-winPlacePerc	(Target variable) 

📈 5. Results and Insights

🧩 Model Results

1)The LSTM model successfully learned sequential relationships between gameplay metrics and win outcomes.

2)It achieved:

-Mean Absolute Error (MAE): 0.045

-Mean Squared Error (MSE): Low and stable across epochs

-R² Score: 0.91

3)The training and validation loss curves converged smoothly, indicating no overfitting and good generalization.

Gameplay Insights

1)Players with high kills, damageDealt, and walkDistance showed a strong correlation with winning.

2)Players who covered more ground (walking or riding vehicles) tended to survive longer and had higher win probabilities.

3)boosts and heals usage indicated good resource management and increased survival chances.

4) kills, damageDealt, and walkDistance as the most significant predictors of success.

5)The LSTM model captures temporal dynamics, showing that early kills and looting influence late-match performance.
