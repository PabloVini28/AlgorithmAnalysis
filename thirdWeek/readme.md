# Solving Recurrences 📐
  - Definition:
    - Recurrences often appear in the analysis of recursive algorithms, expressing the cost of solving a problem in terms of the cost of solving smaller subproblems. Three common methods for solving recurrences are the iterative method, recurrence tree, and master theorem.
## Iterative Method 🔄
  - This approach involves repeatedly expanding the recurrence until a pattern emerges or the base case is reached.
  - Steps:
    - Expand the recurrence step by step.
    - Identify a general formula for the terms.
    - Sum the terms and simplify.
## Recurrence Tree 🌳
  - This method visualizes the recurrence as a tree where each node represents the cost of a subproblem.
  - Steps:
    - Draw the first level of the tree with the original problem size.
    - Split the problem into subproblems and assign costs recursively.
    - Sum the costs at each level.
    - Add up the costs of all levels for the total complexity.
## Master Theorem 📘
  - A direct approach for solving recurrences of the form:
  - T(n)=aT(𝑛/b)+f(n), where a≥1, b>1, and f(n) is an asymptotically positive function.
  - Steps:
    - Compare f(n) with n logba:
    - If f(n)=O(n log b a−ϵ) : T(n)=Θ(n log ba).
    - If f(n)=Θ(n log b a) : T(n)=Θ(n log balogn).
    - If f(n)=Ω(n log b a+ϵ): T(n)=Θ(f(n)).
