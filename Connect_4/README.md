# Building a Connect 4 Agent

## About this Project

The goal of this project was to explore different search and optimization methods to create an agent that can successfully play the classic board game Connect 4. This project also builds off the concepts learned in the n_queens, maze, and robot_vacuum projects. 

## Data & Dependencies

This project utilizes certain helper functions provided by the professor such as a function to visualize the board. Additionally, I use JupyterNotebook to write my code.

## Technical Approach

I apply minimax search with alpha-beta pruning, move ordering, minimax search with alpha-beta pruning with an added depth cuttoff, and pure Monte Carlo search. The final model I land on uses minimax search with alpha-beta pruning with a depth cuttoff. This model also utilizes the best first move found by my Monte Carlo search.

## Highlights
* Model based agent
* Minimax search
* Alpha-beta pruning
* Monte Carlo search

## Conclusion
After building and experimenting with the different search algorithms, I successfully created an agent to efficiently play Connect 

