# Embodied-carbon-cost-and-size-analysis-for-optimal-water-network-design-in-buildings-
This Python script implements the Simulated Annealing optimization algorithm to determine the optimal pipe diameter that minimizes cost while adhering to engineering constraints, such as velocity and pressure loss limits.

How It Works:

Initialization: The algorithm starts with a randomly selected pipe diameter within a predefined range.
Cost Evaluation: The cost function considers material cost and various penalty factors.
Constraints Verification: Each iteration ensures that the velocity remains between 0.3 and 3 m/s, and pressure losses do not exceed 10% of the pipe length.
Temperature-Based Search: The algorithm iteratively explores new solutions by adjusting the pipe diameter, accepting suboptimal solutions probabilistically to escape local minima.
Convergence: As temperature decreases, the search narrows, refining the solution.
