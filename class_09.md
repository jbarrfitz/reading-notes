# Class 09

**Date Due:** April 15, 9 am PDT

## Reading

- [_Dunder Methods_](https://dbader.org/blog/python-dunder-methods)
- [_Statistics - Probability_](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)

## Videos

- [_Intro to Statistics_](https://www.youtube.com/watch?v=MdHtK7CWpCQ)
- [_AI Guru makes $238,800 with misleading paid course. doesn’t credit developers_](https://www.youtube.com/watch?v=7jmBE4yPrOs)

### Reading Questions

#### What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method

Dunder methods provide some baseline functionality for classes that you create. ```python __init__``` for example
is the initialization method for the class, and it contains the constructor for the class. ```python __str__``` is another
common method that provides your class with a string representation whenever you use the print() or str() methods. You
can use these to determine what to do when comparing objects based on the class (for example, determining what makes one
object 'greater' than another).

#### In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?

The main issue is that he outright used others' work without attribution. By failing to properly attribute the work to those
who created it, he essentially was misleading people into believing that he wrote the code. If he needed to use another developer's
code, he should have forked the repo, leaving the history intact, and properly attributed the code to its author.

#### Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation

The statistics module contains many standard statistic methods that you can perform on data sets, such as mean, mode,
median, etc. While it is not a full-fledged statistics library used by data scientists, it does perform many of the basic
statistical functions that might often be needed by a developer.

One example is the median, which in statistics represents the "middle" point in a group of data points, i.e., there are as many
data points below that number as there are above that number.

```python
    from statistics import median
    sample_data = [2, 3, 3, 4, 4, 5, 5, 6, 6, 7]
    print(median(sample_data)) // prints 4.5 to the console
```
