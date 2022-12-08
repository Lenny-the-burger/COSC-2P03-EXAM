# Recursion

-   Chapter 1 covers the topic of recursion.
-   Understand the rules for recursion, including the base case and the progress towards the base case.
-   Be able to determine when recursion should be used and when it should be avoided.
-   Know the time complexity of recursive algorithms, and be able to convert recursive algorithms to iterative algorithms and vice versa.
-  See [Recursion](Recursion.md) for more details

Recursion is a method of solving a problem by defining a function that calls itself with simpler input values until it reaches a base case, at which point it can be solved directly. This allows for a divide-and-conquer approach to problem solving, where a complex problem is divided into smaller subproblems that can be solved independently and then combined to solve the original problem.

## The rules of recursion

There are two key rules that must be followed when using recursion:

-   The base case: the base case is the simplest form of the problem that can be solved directly without the need for further recursion. For example, in a recursive function that calculates the factorial of a number, the base case would be the factorial of 0, which is 1.
-   Making progress towards the base case: every recursive call to the function must make progress towards the base case. This means that the input values to the function must be simplified in some way so that eventually the base case is reached and the function can be solved directly. For example, in a recursive function that calculates the factorial of a number, the input value would be simplified by decrementing the number on each recursive call, until the base case is reached and the function can be solved directly.

## When recursion should be used

Recursion is a powerful tool for solving problems, but it's not always the best approach. In general, recursion should be used when:

-   The problem can be divided into smaller subproblems that can be solved independently and then combined to solve the original problem.
-   The solution to the problem can be expressed in terms of a recursive function that calls itself with simpler input values until it reaches a base case.
-   The problem can be solved directly at the base case without the need for further recursion.

Recursion should be avoided when:

-   The problem cannot be divided into smaller subproblems that can be solved independently.
-   The solution to the problem cannot be expressed in terms of a recursive function.
-   The problem cannot be solved directly at the base case and requires further recursion.

## Time complexity

The time complexity of a recursive algorithm is the number of operations it takes to solve the problem as a function of the input size. In general, the time complexity of a recursive algorithm is determined by the following factors:

-   The time complexity of the base case: the time complexity of the base case is the number of operations required to solve the problem directly at the base case. For example, in a recursive function that calculates the factorial of a number, the time complexity of the base case would be constant because it only requires one operation to return the value 1.
-   The number of recursive calls: the number of recursive calls is the number of times the function calls itself before reaching the base case. For example, in a recursive function that calculates the factorial of a number, the number of recursive calls would be equal to the input value minus 1 because the function calls itself once for each value from 1 to the input value.
-   The time complexity of each recursive call: the time complexity of each recursive call is the number of operations required to simplify the input values on each call to the function. For example, in a recursive function that calculates the factorial of a number, the time complexity of each recursive call would be constant because it only requires one operation to decrement the input value.

## Conversion from/to iterative

Recursive algorithms can often be converted to iterative algorithms, which use loops instead of recursive function calls to solve a problem. This can be useful in cases where recursion is not appropriate, such as when the problem cannot be divided into smaller subproblems or when the solution cannot be expressed in terms of a recursive function.

To convert a recursive algorithm to an iterative algorithm, the following steps can be followed:

1.  Identify the base case and the progress towards the base case in the recursive algorithm.
2.  Create an iterative loop that starts with the initial input values and continues until the base case is reached.
3.  Inside the loop, implement the progress towards the base case by applying the necessary operations to the input values on each iteration.
4.  Once the base case is reached, return the result of the algorithm.

Conversely, it's also possible to convert an iterative algorithm to a recursive algorithm. To do this, the following steps can be followed:

1.  Identify the initial input values and the loop conditions in the iterative algorithm.
2.  Create a recursive function that takes the initial input values as arguments.
3.  Inside the function, check if the loop conditions have been met. If they have, return the result of the algorithm.
4.  If the loop conditions have not been met, apply the necessary operations to the input values to make progress towards the base case and then call the function recursively with the updated input values.
5.  Once the base case is reached, return the result of the algorithm.

Overall, understanding how to convert recursive algorithms to iterative algorithms and vice versa can be useful in situations where one approach is more appropriate than the other.
