##  Linear Programming using Gurobi Optimization & Python's inbuilt Scipy 

<img target="_blank" src="https://github.com/dipakml/Linear-Programming-using-Gurobi-Optimization-Python-s-inbuilt-Scipy-/blob/master/gurobi.jpeg" width=800>

### Table of Content
  * [Overview of Linear Programming](#overview)
  * [Problem Statement](#problem-statement)
  * [Solving using Python's inbulit Scipy](#using-scipy)
  * [Solving Using Gurobi Optimization](#gurobi-optimization)




### Overview of Linear Programming 
Optimization is the process of finding maximum or minimum value of a given objective by controlling a set of decisions in a constrained environment. In simple words, an optimization problem consists of maximizing or minimizing a real function by systematically choosing input values from within an allowed set and computing the value of the function.

The real function (objective function) can be the cost of delivering goods from a warehouse to its customers which we would like to minimize by choosing the optimal route and optimal set of vehicles (decision variables) to deliver the goods given a limited number of drivers and time (constraints). This is a generic case of Route Optimization in the world of Operations Research and Optimization.

Another very famous problem in the field of Computer Science is TSP or Travelling Salesman Problem, wherein we want to find the shortest route or least costly route to travel across all cities, given the pairwise distances between them. In this case, our objective function becomes minimizing the total distance (or total cost) travelled, decision variables become binary variables which tell whether the traveller should travel from City i to City j and constraints are applied such that the traveller covers all the cities and does not visit a city twice. We will also be handling a simpler but similar kind of problem today.


###  Problem Statement



### Solving using Python's inbulit Scipy

**Note-** Scipy linprog() solves only minimization (not maximization) problems and doesn’t allow inequality constraints with the greater than or equal to sign (≥). To work around these issues, you need to modify your problem before starting optimization:

Instead of maximizing z = x + 2y, you can minimize its negative(−z = −x − 2y).
Instead of having the greater than or equal to sign, you can multiply the yellow inequality by −1 and get the opposite less than or equal to sign (≤).

After introducing these changes, you get a new system:




### Solving Using Gurobi Optimization
The Gurobi Optimizer is a state-of-the-art solver for mathematical programming. The solvers in the Gurobi Optimizer were designed from the ground up to exploit modern architectures and multicore processors, using the most advanced implementations of the latest algorithms.

First we need to install gurobipy using pip install:
Open cmd & type pip install gurobipy
OR
In Jupyter notebook type !pip install gurobipy



Next steps:
- Create a new model
- Create variables
- Set objective function
- Add constraints
- Solve



### Technologies Used  
![](https://forthebadge.com/images/badges/made-with-python.svg) 

<img target="_blank" src="https://github.com/dipakml/Prediction-of-Concrete-Compressive-Strength/blob/master/Logo_Images/streamlit.png" width=160>


