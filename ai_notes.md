Week :1 
What is AI:
It covers the wide varieties of techniques. Anytime a computers or systems do something or appear intelligent 
or rational in some way like being able to play game than people can or being able to understand human language and respond back to us.

Search:
Learning:
Neural Networks:
Language:

Search:

Maps is an AI algorithm 

Agent: Entity that perceives that environment and acts upton that environment. For example an car
State: Configuration between the stages in the environment
Initial stage: Where the agent will start 
Actions: Choices to take during the states 
Transition model: a description of what state results from performing any applicable action in any state
results(s, a)
state space: the state of all states reachable from the initial state by any sequence of actions
goal test: a state to determine the state is a goal test
path cost: Numerical cost of taking any action 

Search problems:
Initial State
actions
transition model
goal test
path cost function 

Solution: Sequence of actions that lead from initial state to the goal state

Node:
It is a data structure that keeps track of ä
* a state
* a parent
* an action
* a path to cost

Frontier: All the data structure we could explore next but have not explored

Approch:
* Start with a frontier that contains the initial state
Repeat:
	- if the frontier is empty then there is no way to reach the goal
	- Else: remove a node from the frontier
	- if node contains the goal test, found the solution.
	- else, expand the node, add resulting nodes to the frontier 
	
Revisedm Approch:
* Start with a frontier that contains the intial state
* Start with an empty explored state
	- if the frontier is empty then there is no way to reach the goal
	- Else: remove a node from the frontier
	- if node contains the goal test, found the solution.
	- else, add the node to the explored state 
	- expland the node, add resulting nodes to the frontier if they arent already
	in the frontier or the expolred state

Statck:
One of the simplest way to add and remove the node from the data structure 
last-in and first-out data type

Breadth First Search: BFS
* It expands the swllowest node. Explore the all possible point
* It uses FIFO(first in first out)

Depth first Search: DFS
* When it reaches the dead end it chooses different nodes 
* This search is more stable and will find a solution
* When it reaches the dead end it chooses different nodes 
* Memory saving

Uninformed Search:
Search Algorithm that uses no problem specific knowdlege 

Informed Search: Search stratergy that uses problem specfic knowdlege to
find the solution

Greedy best-first search:
Search based algorithm that expands the node close to the goals as estimated
by the heuristic function h(n).
It uses the estimation

A * search:
search algorithm that expands node with lowest value of
g(n) + h(n)
g(n) * cost to reach the node
h(n) * estimated cost to goal, heuristic function
h (n): should always be under estimating, it should be more consistent 

Adversial Search:
MinMax:
Depth limited Minimax