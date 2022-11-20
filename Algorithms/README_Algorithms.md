# Algorithms

- A set of instructions to complete a task.
- In other words: Input Data --> Caluculation --> Stop when answer found.

- What makes agood algorithm?
- - Correctness
- - Efficiency.

- Big O
- Big O is used to define the efficiency of an algorithm.

- Time Complexity: A way of showing how the runtime of a function increases as the size of input increases.

- Indicator for calculating Big O of an algorithm:
- If the algorithm is in the form `do this, then you are all done, do that`, then one add the runtime.

```java
Add the runtime: O(A+B)
Example: One for loop followed by another for loop
```

- If the algorithm is in the form `do this for each time you do that`, then one multiply the runtime.

```java
Multiply the runtime: O(A*B)
Example: One for loop which contains another for loop within itself
```

## Guidelines for measuring Big O

![Guidelines for calculating Complexity](https://github.com/syedumerahmedcode/concept-in-simple-words/concept-in-simple-words/blob/master/algorithms/GuidelinesForCalculatingComplexity.jpg)