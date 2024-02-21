# N Queens Local Search

## About this Project

The goal of this project was to use local search to find an arrangement of n queens on an n x n chess board where there are no conflicts between any of the n queens (no queen can take another queen). 

## Data & Dependencies

My project utilizes a number of helper functions given by the professor listed under the "Helper Functions" header in my Jupyter Notebook.

## Technical Approach

I implemented different local search algorithms to minimize the number of conflicts between queens on the board such as steepest-ascent hill climbing, different versions of stochastic hill climbing,  hill climbing search with random restarts, and simulated annealing. 

After creating all of these models, I create a table of the 4x4 board average runtime, 4x4 board average global optimality percentage, 8x8 board average runtime, 8x8 board average global optimality percentage, and the largest board solvable under one-tenth of a second.

## Highlights

* Local search algorithms
* Simulated annealing

## Conclusion

Every algorithm scales poorly with problem size in some way or another. For non random restart algorithms (aside from simulated annealing), the runtime for the smaller board was rather low, however, the accuracy of finding an optimal solution was also low. Whenever the board size increases from 4x4 to a full size chess board at 8x8, the accuracy drops even lower to sub 15% for ever algorithm. The low accuracy makes sense since for the non random restart algorithms, it is very easy for these algorithms to get stuck in a local optimum. Simulated annealing has the highest global accuracy for the 8x8 board. This is caused by the temperature schedule that allows simulated annealing to escape local optima.

The random restart algorithms scale poorly in a different way than the non random restart algorithms. Unlike the non RR algorithms, the RR algorithms achieve a 100% accuracy rating (aside from the random restart first choice algorithm and the random restart simulated annealing algorithm). This is because, the RR algorithms randomize the initial starting state. This reduces the chance of getting caught in a local optimum given the rules the algorithm is confined by. This 100% accuracy continues even when the size of the board increases from 4x4 to 8x8. However, the runtime for each RR algorithm increases dramatically. My guess as to why the simulated annealing does not perform well with random restarts is because it essentially already accommodates variability with the temperature schedule. Whenever you add more randomization to the mix, the accuracy decreases.
