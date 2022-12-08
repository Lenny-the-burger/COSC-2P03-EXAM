-   Chapter 7 covers the topic of sorting.
-   Know how to implement and compare the following sorting algorithms:
    -   Heapsort (both ways)
    -   Quicksort, including the choice of pivot
    -   Mergesort
    -   Radix sort

Sorting is the process of arranging a collection of items in a specific order, such as ascending or descending order. Sorting is a common operation in many applications, and there are many different algorithms that can be used to sort a collection of items.

## Heapsort

Heapsort is a sorting algorithm that uses a max-heap or min-heap to sort a collection of items. It works by building a heap from the input collection, then repeatedly removing the maximum or minimum value from the heap and adding it to the output collection.

There are two ways to implement heapsort:

-   In-place heapsort: an in-place heapsort builds the heap in-place, using a portion of the input array for the heap. This approach is efficient because it uses a constant amount of additional memory, but it is more complex to implement because it requires the input array to be modified in-place.
-   Out-of-place heapsort: an out-of-place heapsort builds the heap using a separate array, then copies the sorted items from the heap to the output array. This approach is simpler to implement than in-place heapsort, but it requires additional memory to store the heap.

## Quicksort

Quicksort is a sorting algorithm that uses the divide-and-conquer approach to sort a collection of items. It works by dividing the input collection into two or more subcollections, then sorting each subcollection and merging the sorted subcollections back together to form the output collection.

One of the key decisions in implementing quicksort is choosing the pivot element, which is the element around which the input collection is divided. There are several different strategies for choosing the pivot element, including:

-   Choosing the first element in the input collection as the pivot.
-   Choosing the last element in the input collection as the pivot.
-   Choosing a random element in the input collection as the pivot.
-   Choosing the median element in the input collection as the pivot.

The choice of pivot element can have a significant impact on the time complexity of quicksort, so it's important to choose an appropriate pivot strategy for the specific input data.

## Mergesort

Mergesort is a sorting algorithm that uses the divide-and-conquer approach to sort a collection of items. It works by dividing the input collection into two or more subcollections, then sorting each subcollection and merging the sorted subcollections back together to form the output collection.

Mergesort is a stable sorting algorithm, meaning that items with the same value are preserved in their original order in the output collection. This property can be useful in some applications, such as when sorting a collection of records that contain multiple fields.

## Radix sort

Radix sort is a sorting algorithm that uses the digits of the items being sorted to determine their relative order. It works by sorting the items based on their least significant digit, then sorting them again based on their next least significant digit, and so on until all the digits have been considered.

Radix sort is a non-comparison sorting algorithm, meaning that it does not use comparisons between items to determine their order. This makes it more efficient than comparison-based sorting algorithms in some cases, but it is only applicable to collections of items that can be represented as integers or strings with a fixed number of digits.

## Comparison of sorting algorithms

There are many different sorting algorithms, and the appropriate algorithm to use will depend on the specific requirements of the application. Some factors to consider when comparing sorting algorithms include:

-   Time complexity: the time complexity of a sorting algorithm is the amount of time it takes to sort a collection of items as a function of the number of items in the collection. Some sorting algorithms are more efficient than others, so it's important to choose an algorithm with a time complexity that is appropriate for the size of the input data.
-   Space complexity: the space complexity of a sorting algorithm is the amount of memory it requires to sort a collection of items as a function of the number of items in the collection. Some sorting algorithms are more space-efficient than others, so it's important to choose an algorithm with a space complexity that is appropriate for the size of the input data and the available memory.
-   Stability: a stable sorting algorithm is one that preserves the relative order of items with the same value in the output collection. This property can be useful in some applications, such as when sorting a collection of records that contain multiple fields.
-   Adaptability: an adaptive sorting algorithm is one that can take advantage of pre-existing order in the input collection to sort the items more efficiently. This can be useful in some cases, such as when sorting a collection of items that is mostly sorted but has a few out-of-order items.
-   Special properties: some sorting algorithms have special properties that make them suitable for specific applications. For example, radix sort is a non-comparison sorting algorithm, which makes it more efficient than comparison-based algorithms in some cases.