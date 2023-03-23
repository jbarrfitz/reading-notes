# Prep - Data Structures & Algorithms

**Date Due:** March 18, 11:59pm PDT

Data structures and algorithms are extremely important for a software developer, as a thourough understanding
of which of these is appropriate for a particular problem will lead to far more efficient coding. If the correct
algorithm is selected, valuable resources are less likely to be wasted.

## Video

- [_Basic Recursion_](https://www.youtube.com/watch?v=vPEJSJMg4jY)
- [_Data Structures in 15 Minutes_](https://www.youtube.com/watch?v=sVxBVvlnJsM)
- [_Big O Explained_](https://www.youtube.com/watch?v=v4cd1O4zkGw)

## Reading

- [_Basic Data Structures_](https://towardsdatascience.com/8-common-data-structures-every-programmer-must-know-171acf6a1a42)
- [_Why Big O?_](https://triplebyte.com/blog/why-you-should-learn-big-o-and-stop-hacking-your-way-through-algorithms)

## Discussion Questions

### What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

Data structures have different strengths and weaknesses, so it is important to consider those when
determining which one is most suitable for solving a particular problem. Some data structures,
such as binary search trees, can be very effective when searching for a particular item amongst
a large collection, while linked lists might be more appropriate for problems whose solutions would
require a lot of insertion and deletion amongst the data points.

### How can we ensure that we'll avoid an infinite recursive call stack?

The best way to avoid infinite loops in a recursive function is through the use of a _base case_
designed to stop the recursion whenever a specific point has been met. The recursive function should
only run when the base case has **not** been met.

## Notes

Recursion can be a useful technique in terms of making code easier to understand,
_in some circumstances_. A drawback to this approach, though, is that it is easy
to end up in an infinite loop if the function is not created properly. In addition,
the concepts behind recusion can often be more difficult to wrap your head around.

## Things I would like to know more about

- What circumstances are the most appropriate for the use of linked lists, given their limitations?
- In the real world, is there a tendency to just use _built-in_ functions, like **array.sort()**, rather than seeking out the perfect algorithm?
