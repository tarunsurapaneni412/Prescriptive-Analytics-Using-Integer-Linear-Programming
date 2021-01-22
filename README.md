# Prescriptive-Analytics-Using-Integer-Linear-Programming
# DREAM TEAM SPORTS CONSULTANCY 

Soccer is the most popular game having a huge fanbase across the world. DREAMTEAM  SPORTS CONSULTANCY is a leading team strategy provider and is known for its team  building solutions in the field of soccer. For the upcoming season of Champions league, 3 teams  have together decided to seek assistance from Dream Team Sports Consultancy to build their teams  from a pool of 60 available players. 
Every team has a certain budget (not the same for all teams) wherein they need to build a team  consisting of 2 category players (star players and inexperienced players), a team manager and a  physio. Also, every team has certain requirements when it comes to the type of players.  
⇒ Mid-fielders 
⇒ Defenders 
⇒ Strikers 
⇒ Goalkeepers 
Each category players, managers and physios have a fixed price set to avail their duties. The franchise aims to build the team with minimal spending. 
This project strives to analyze and minimize the total allocation cost of the 3 teams.

# Integer Linear Programming (LP) Model 
Integer linear programming is a branch of linear programming where the only restriction is all the  variables of the model have to be only Integer. The divisibility requirement in this model is that  the non-integer solutions are not allowed. All the other requirements of objective function,  constraints, decision variables, non-negativity, Linear relationship and additivity remain constant.  
There are three types of integer models 
• Pure-integer model where all the decision variables are required to have integer values for the  optimal solution. 
• Zero-One integer model where the variables are restricted to either 0 or 1 (binary variables) • Mixed-integer model involves variables where some are integers, while others can be non integers i.e. binary. 
The algorithm that is used to solve the integer models is the branch and bound method. This method searches for an optimal solution by examining only a small part of the total number of possible solutions. This method starts with solving the model using the Simplex Method (similar to that of  the Linear programming method), in the process if the algorithm finds a non-integer solution, it breaks the area of the feasible solutions into sub problems until the optimal solution is found. If  the solution of a sub problem has a total profit or cost worse than the current feasible bound, it is  discarded, and only the remaining sub problems will be evaluated. At a point where no more  subproblems can be created i.e. all variables are integers the optimal solution is reached. This  model introduces the concept of feasible and infeasible bounds. 

#  Implementation Details 
The Problem statement for this project is to build three teams for a franchise considering the inputs  and requirements proposed by them while minimizing the total budget possible. In this process,  the team may or may not get a player, e.g. team gets a star striker or not, its either 0 or 1 but there  won’t be a situation where they get a fractional value of 1.5 player or a 0.75 player. To satisfy this  condition we chose Integer Linear Programming as this ensures that the above-mentioned situation  of getting decimal values doesn’t arise. 
# Formulation of the model 
The Team Allocation Model provides an optimal allocation of players, managers and physios to  the 3 teams. The main decision that the model needs to make is to allot different category players  of specific types to the 3 teams. These allocations are done in such a way that it minimizes the  total allocation cost to build the 3 teams. 
The Team Allocation Model is an integer linear program with binary values having a set of  constraints which are mainly the requirements placed by the 3 teams and the mandatory allocation  constraints. All these made the Model a large-scale application with 200 decision variables and  100 constraints hitting the maximum limit of the data solver.


