-   Chapter 2 covers the topic of complexity.
-   Know the relative order of common complexity classes: constant, logarithmic, linear, polynomial, and exponential.
-   Be able to express the complexity of a given algorithm using big O notation.
-   Know the complexity of any algorithm studied, as well as possible improvements.

Complexity is the study of the efficiency of algorithms, with the goal of understanding how their performance scales as the input size grows. This is important because, in many cases, the input size to an algorithm can be very large, and the algorithm's efficiency will greatly impact the amount of time and resources it takes to run.

## Know the relative order of common complexity classes

There are several common complexity classes that are used to express the efficiency of an algorithm. These classes are:

-   Constant complexity: an algorithm with constant complexity has a time or space requirement that is independent of the input size. For example, a simple lookup operation in an array has constant complexity because it will always take the same amount of time to execute, regardless of the size of the array.
-   Logarithmic complexity: an algorithm with logarithmic complexity has a time or space requirement that increases logarithmically with the input size. For example, a binary search algorithm has logarithmic complexity because the number of operations it takes to find an element in the array increases logarithmically with the size of the array.
-   Linear complexity: an algorithm with linear complexity has a time or space requirement that increases linearly with the input size. For example, a simple sorting algorithm such as bubble sort has linear complexity because the number of operations it takes to sort an array increases linearly with the size of the array.
-   Polynomial complexity: an algorithm with polynomial complexity has a time or space requirement that increases as a polynomial function of the input size. For example, a more complex sorting algorithm such as quicksort has polynomial complexity because the number of operations it takes to sort an array increases as a polynomial function of the size of the array.
-   Exponential complexity: an algorithm with exponential complexity has a time or space requirement that increases exponentially with the input size. For example, an algorithm that attempts to solve the traveling salesmanperson problem by trying all possible combinations of cities has exponential complexity because the number of operations it takes to solve the problem increases exponentially with the number of cities.

## Be able to express the complexity of a given algorithm

The complexity of an algorithm can be expressed using big O notation. This notation gives an upper bound on the time or space requirement of an algorithm, indicating how it scales as the input size grows.

For example, if an algorithm has a time requirement that is linear in the input size, it can be expressed as O(n), where n is the size of the input. If an algorithm has a time requirement that is quadratic in the input size, it can be expressed as O(n^2), where n is the size of the input.

It's important to note that big O notation only gives an upper bound on the complexity of an algorithm. This means that the actual complexity of the algorithm may be lower than the bound indicated by the notation.

## Know the complexity of any algorithm studied

When studying algorithms, it's important to understand their complexity so that you can make informed decisions about which algorithm to use in a given situation. For example, if you're given a problem that requires sorting a large array, you would want to use an algorithm with a lower time complexity than an algorithm with a higher time complexity, such as quicksort over bubble sort.

## Possible improvements

In many cases, it's possible to improve the complexity of an algorithm by making changes to its design or implementation. For example, a sorting algorithm that has quadratic time complexity can be improved by using a more efficient sorting algorithm, such as quicksort, which has average case time complexity of O(n log n).

Another way to improve the complexity of an algorithm is to use a more efficient data structure. For example, if an algorithm uses an array to store data, it may be possible to improve its time complexity by using a more efficient data structure such as a binary tree or a hash table.

It's also possible to improve the complexity of an algorithm by using more efficient algorithms for subproblems. For example, if an algorithm solves a problem by dividing it into smaller subproblems and solving each subproblem independently, it may be possible to improve its time complexity by using more efficient algorithms to solve the subproblems.

Overall, understanding the complexity of an algorithm and identifying potential improvements can help you design and implement more efficient algorithms.