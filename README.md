# Analyzing Win Probabilities in the Dice Game "Liar's Dice" Using Monte Carlo Simulations
## Project Overview
This project simulates and analyzes the dice game Liar's Dice using Monte Carlo simulations. The primary objective is to explore how different player strategies and rule changes impact gameplay outcomes. Additionally, the project aims to validate the fairness and randomness of the game mechanics.
Project Type: Type II - Original Monte Carlo Analysis 

## Team Members:
Yueyue Lin, GitHub: https://github.com/Yena830
Jiajing Liang, GitHub: https://github.com/Fiona729



## Game Overview
Players bid on dice outcomes, considering both quantity and face value.
Players may challenge the previous bid by calling "Liar!" The game dynamics depend on the validity of the challenge.
Special rules:
"1" acts as a wildcard, contributing to any face value.
The player who loses the challenge is penalized (e.g., by losing a die).
![image](https://github.com/user-attachments/assets/33a0e221-4f8b-4819-907b-95f4aa4ac5a4)

Code Design
The project is structured into modular Python scripts to enable flexibility and scalability. The key components include:

1. Game Engine: game_play_rule.py
Implements core gameplay mechanics such as:
roll_dice(): Simulates dice rolling.
valid_challenge(): Checks if a "Liar" call is valid.
update_all_dice(): Updates dice counts after each round.
simulate_game(): Executes the entire game loop.
2. Player Strategies: game_strategies.py
Defines strategies used by players during simulations:
random_bid(): Generates random bids.
inform_bid(): Prioritizes bids based on preferred dice.
make_action(): Decides whether to bid or call "Liar" based on thresholds.
3. Validation Tools: validation_setting.py
Evaluates the fairness and correctness of the gameplay:
Win rate analysis.
Validation of dice randomness.
Heatmaps and data visualizations.
4. Experiments and Visualizations: Jupyter Notebook
Integrates the core modules for hypothesis testing and result visualization.


## Hypotheses
The project tests several hypotheses related to gameplay dynamics and strategies:

1. First Caller Advantage: The first player has a higher win rate due to their ability to set the initial bid.
2. Preferred Dice Bid: Players bidding based on their most frequent dice achieve higher win rates.
3. Threshold for Calling "Liar": Players using optimized thresholds for challenges outperform those using random strategies.
4. Optimal Strategy Combination: Combining threshold-based and preferred dice bidding yields the best outcomes.
5. Special Rule Impact: Modifications to the rules (e.g., reducing one die instead of eliminating a player) affect fairness and strategy effectiveness.


## Validation
To ensure the robustness of the simulations, the following validations were conducted:

1. Dice Distribution: Verified that dice rolls follow a uniform distribution.
2. Challenge Distribution: Confirmed players' challenge behavior aligns with expectations under random strategies.
3. Random Strategy Outcomes: Demonstrated uniform win rates across players when no strategy is applied.

## How to run
Clone this repository.
Run the notebook.

