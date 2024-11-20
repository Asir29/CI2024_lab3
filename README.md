# CI2024_lab3
Lab3 for Computational Intelligence Course at Polito

The approach for the n-puzzle has been understood from the lectures. The road is in the following lines.  
The initial random state has been provided by the professor.  
The goal is to arrange a NxN grid in sequential order, with an empty slot (represented by 0) in the final position.  
The program:  
-Applies Beam Search with a specified beam size to retain only the most promising moves.  
-Prioritizes moves by their closeness to the goal using a priority queue.  
Key Components:  
-Beam Size: Limits the number of states explored at each step, improving efficiency.  
-Priority Queue: Keeps track of puzzle states by priority, defined as the distance from the goal.  
-Visited Set: Prevents redundant state evaluations

# Suggested parameters for priority estimation:  
N = 3, 4 only difference_from_goal is sufficient  
N = 5 use 80% difference and 20% Manhattan distance 
