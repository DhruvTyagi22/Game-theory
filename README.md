# Game Theory Simulations

A collection of Python-based simulations and visualizations exploring core concepts in Game Theory. This repository models strategic interactions, equilibrium thresholds, and repeated games using computational methods.

Projects
1. Bayesian Equilibrium: The Director-Actor Game 

File: director_actor_bayesian_game.ipynb

This notebook models a Bayesian Game (Game of Incomplete Information). It simulates a scenario between a Director (who can be either Strict or Lenient) and an Actor (who must decide between High or Low effort).

    Key Concept: Bayesian Nash Equilibrium.

    Mechanism: Calculates the expected cost for the Actor based on their belief (p) that the Director is "Strict."

    Visualization: Plots the cost functions for "Safe" vs. "Gamble" strategies and identifies the equilibrium threshold (p∗)—the tipping point where the optimal strategy changes.

    Parameters: Adjustable costs for High/Low effort (CH​,CL​) and discount factors (δ).

2. Repeated War Game (Iterated Prisoner's Dilemma) 

File: Repeated_Prisoner’s_Dilemma–style_war_game.ipynb

A simulation of an Iterated Prisoner's Dilemma, framed as a "War Game" played over a series of days. This project allows users to test various classic Game Theory strategies against a dynamic opponent.

    Key Concept: Repeated Games, Cooperation vs. Defection, and Discounted Payoffs.

    The Twist: The simulation includes a forced "Betrayal Event" at the midpoint of the game to test how different strategies recover (or fail to recover) from broken trust.

    Implemented Strategies:

        Tit-for-Tat: Reciprocates the opponent's previous move.

        Grim Trigger: Cooperates until betrayed once, then defects forever.

        Tit-for-Two-Tats: Forgiving; requires two attacks to retaliate.

        Always Defect: Aggressive "Hawk" strategy.

        Mad Man: Random decision-making.

    Output: Generates a pandas DataFrame of results and bar charts comparing the User Score, Enemy Score, and the "Perfect Peace" benchmark.
