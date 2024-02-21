# Maze Solving Agent

## About this Project

The goal of this project was to implement different search algorithms to successfully have a goal based agent get from the start point of a maze to the desired end. The maze agent works its way through a maze environment represented by an array. The maze is assumed to be deterministic, discrete, and known. My algorithms use search trees and the node class to search the possible routes through the maze. The chosen routes and methodology in finding these routes depends on the respective search algorithm.

## Data & Dependencies

This project utilizes maze txt files to load in different maze designs and the maze_helper.py file to access helper functions.

## Technical Approach

Uninformed search algorithms:
Breadth First Search and Depth First Search

Informed search algorithms: 
Greedy Best First Search and A* search with Manhattan distance as the heuristic for both algorithms.

After building my search algorithms, I ran experiments to find the average path cost, number of nodes expanded, max tree depth, max number of nodes in memory, and max frontier size for each algorithm across each maze variation. Additionally, I visualized the cost and number of nodes expanded using boxplots.

Lastly, I built an Iterative Depth First Search and ran my search algorithms on mazes with multiple end goals.

## Highlights
* Search trees
* Search algorithms
* Goal based agent

## Conclusion

There are some interesting findings after running an experiment comparing the depth reached for BFS, DFS, and IDS with the multigoal mazes. BFS finds the first goal at a lesser depth than the other two algorithms. However, as we have learned, BFS is expensive to implement since it requires high storage and high run time. Conversely, DFS finds the first goal at a higher depth, but DFS does not have the same high storage cost that BFS has. The middle ground between these two algorithms is IDS since it iterates through paths at each depth until a solution is found. Therefore, it finds the solution at a lesser depth than DFS while also not having the same large storage requirements as BFS.

