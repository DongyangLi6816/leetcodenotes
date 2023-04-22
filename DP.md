# Dynamic Programming
## When to use DP
- The problem can be broken into overlapping subproblems(reuseable).
- The problem asks for an optimal solution that can be formed from smaller problems - maximum, minimum, number of ways...
- future decisions depend on the ealier decisions.
## Framework for DP
```
You are climbing a staircase. It takes n steps to reach the top.

Each time you can either climb 1 or 2 steps. In how many distinct ways can you climb to the top?
```
- Define the state - set of varibles that can sufficiently describe a scenario.
    - Eg. the current step we are on. i
    - Every unique value of i represents a unqiue state.
- A function that compute the answer to the problem for every given state.
- A recurrence relation to transition between states.
    - An equation that relates different states with each other.
        - We either climb to 30th stair through 28th or 29th stair. dp(30) = dp(28)+dp(29).
- A base step
    - What states can I find the answer to without using dp?

- Top down - start from the target and recursive down - hashmap
- Bottom up - start from the base case and use for loop to iterate up - array