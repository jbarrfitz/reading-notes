# Class 08

**Date Due:** April 11, 6:30 pm PDT

## Reading

- [_List Comprehensions_](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
- [_Primer on Decorators_](https://realpython.com/primer-on-python-decorators/)

### Reading Questions

### What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers

List comprehension is similar to using a for loop, but makes it much more compact, and it offers you the ability to use a filter
when creating the list. The basic syntax is:

```python
    list_name = [expression for item in list if condition]
```

With this basic syntax, you simply supply an expression you wish to perform on the list of items you are working
with, supply the list (which could be a range, a string, or any other iterable object), and provide conditions if
you wish to qualify which items should be placed in the new list.

Example: list comprehension that squares the elements in a given list of integers

```python
old_list = [23, 32, 45, 63, 119]
new_list = [number ** 2 for number in old_list]
print(new_list)
```

The result is [529, 1024, 2025, 3969, 14161]

### What is a decorator in Python?

Decorators are essentially functions that are used to modify the way that
other functions work. They act as wrappers around the functions and often
incorporate some special behavior. An example of this is the @pytest.mark.skip
decorator that allows you to skip a test in a Pytest suite of tests.

### Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading

Decorators can modify behavior by changing the way that functions work. You use
the @ symbol to indicate their presence, and they often what a function output or
changes the behavior in some way as to make them useful for special purposes. One
example of this is a timer function, in which case a specially-designed decorator
can help you understand how long a function takes to run, which could be useful in
debugging your code and spotting where issues might arise. A timer example from our
text:

```python
import functools
import time

def timer(func):
    """Print the runtime of the decorated function"""
    @functools.wraps(func)
    def wrapper_timer(*args, **kwargs):
        start_time = time.perf_counter()    # 1
        value = func(*args, **kwargs)
        end_time = time.perf_counter()      # 2
        run_time = end_time - start_time    # 3
        print(f"Finished {func.__name__!r} in {run_time:.4f} secs")
        return value
    return wrapper_timer

@timer
def waste_some_time(num_times):
    for _ in range(num_times):
        sum([i**2 for i in range(10000)])
```

The decorator serves as a "wrapper" around the function that can be used whenever
you invoke the '@timer' decorator when calling the function that is wrapped inside
of it.
