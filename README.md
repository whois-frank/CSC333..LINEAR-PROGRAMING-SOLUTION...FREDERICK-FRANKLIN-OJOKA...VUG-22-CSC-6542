# CSC333..LINEAR-PROGRAMING-SOLUTION...FREDERICK-FRANKLIN-OJOKA...VUG-22-CSC-6542FREDERICK FRANKLIN OJOKA

VUG/22/CSC/6542











Here's a detailed README file for the Python code, including instructions on running it and explaining the methodology:





---



Linear Programming Solver - Maximization and Minimization Problems



Overview



This repository contains Python code to solve various linear programming (LP) problems using the SciPy library. The problems involve maximizing or minimizing an objective function subject to a set of linear constraints. The code also generates visualizations, such as graphs with shaded feasible regions and optimal solutions.





---



Methodology



The code employs the following steps for solving each problem:



1. Define the objective function: We either aim to maximize or minimize a linear objective function, typically in the form:







c_1 x_1 + c_2 x_2 + ... + c_n x_n



2. Set up constraints: Constraints are linear inequalities or equalities that limit the values of the decision variables:







A x \leq b



3. Solve the problem:



SciPy's linprog function is used to solve the linear programming problem.



The function finds the optimal solution that maximizes or minimizes the objective function, depending on the problem's nature.







4. Identify corner points:



Corner points (vertices) of the feasible region are determined by solving pairs of constraints to find their intersection points.



These points are filtered to ensure they satisfy all the constraints, and only feasible corner points are considered.







5. Visualize the feasible region:



Constraints are plotted as lines, and the feasible region is shaded.



Feasible corner points are marked with green dots, and the optimal solution (found by linprog) is marked with a red dot.











---



Requirements



To run the code, you need to have Python installed, along with the following packages:



NumPy: for numerical operations.



Matplotlib: for plotting graphs.



SciPy: for linear programming functions.





Install Required Libraries



If you don’t have the required libraries installed, you can install them using pip:



pip install numpy matplotlib scipy





---



Running the Code



Steps to Run the Python Code



1. Clone the repository or download the Python script (e.g., lp_solver.py).





2. Run the script:



Open a terminal or command prompt.



Navigate to the directory where the script is located.



Execute the script using Python:





python lp_solver.py



The script will solve 10 different linear programming problems and display the results, including optimal solutions and graphs showing the feasible region and corner points.









---



Problems Solved



1. Maximizing Profit for a Factory



Objective: Maximize profit by producing products A and B, with given machine time and raw material constraints.



2. Minimizing Cost for a Manufacturer



Objective: Minimize production cost for products X and Y, given labor and material constraints.



3. Maximizing Production with Multiple Resources



Objective: Maximize profit by producing two products with constraints on labor, material, and machine time.



4. Maximizing Revenue from Sales



Objective: Maximize revenue from two products, considering advertising costs and production capacity.



5. Resource Allocation for Two Projects



Objective: Maximize profit by allocating labor and capital to two projects.



6. Production Planning for a Bakery



Objective: Maximize profit by producing chocolate and vanilla cakes with constraints on baking time and flour.



7. Minimizing Cost for a Transport Company



Objective: Minimize the transport cost using two types of vehicles with constraints on fuel and driver time.



8. Maximizing Revenue from Two Products



Objective: Maximize revenue by producing two products, considering labor, raw material, and machine time constraints.



9. Advertising Campaign Budget Allocation



Objective: Maximize reach by allocating an advertising budget between two campaigns with specific media constraints.



10. Meal Planning for a School Cafeteria



Objective: Plan a meal schedule to maximize the number of meals served, considering the ingredients available.





---



Output



For each problem, the following outputs will be provided:



Optimal Solution: The optimal values of the decision variables.



Feasible Corner Points: The corner points that satisfy all constraints.



Graph: A plot showing:



Constraints as lines.



Feasible region shaded.



Feasible corner points as green dots.



The optimal solution as a red dot.









---



Code Explanation



find_corner_points: Finds the intersection points of the constraint lines by solving the system of linear equations.



filter_feasible_points: Filters out the infeasible points that do not satisfy all constraints.



plot_graph: Plots the graph of constraints, feasible region, and optimal solution.



solve_problem: Solves the linear programming problem using linprog, calculates corner points, and visualizes the solution.





Each problem is solved by calling the solve_problem function with the appropriate parameters (objective coefficients, constraints, and bounds).





---



Example of Output



For each problem, the output will look something like:



Maximizing Profit for a Factory

Optimal Solution:  [2. 2.]  # Solution (x=2, y=2)

Feasible Corner Points: [[2. 2.], [0. 4.], [4. 0.]]



Additionally, a plot will be generated showing the constraints, feasible region, and the optimal solution.





---



Troubleshooting



If you encounter any issues while running the code:



Make sure all required libraries are installed (numpy, matplotlib, and scipy).



Check that your Python version is 3.x (recommended version: 3.7+).



Ensure that the terminal or IDE you're using is properly set up to execute Python scripts.







---



Conclusion



This repository provides a useful tool for solving linear programming problems, with visualizations to better understand the feasible region and optimal solutions. The code is flexible and can be adapted for other LP problems by modifying the objective function, constraints, and bounds.





---

 

