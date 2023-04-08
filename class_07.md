# Class 06

**Date Due:** April 8, 9 am PDT

## Reading

- [_Python Scope_](https://realpython.com/python-scope-legb-rule/)

## Video

- [_Big O Notation is Simpler than You Might Think_](https://www.youtube.com/watch?v=dNorFNlDbX0)

### Reading Questions

#### Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both

Variable scope in Python is the concept of specificity in terms of where variables are available, based on where
they are created. Global variables are defined outside of any function and are thus available throughout the
program. These variables can be accessed or modified by any part of the code. Local variables are defined within
the function, and are only available within that function. Multiple local variables can have the same name, within
their own separate functions, for example, and those variables are only available within the functions in which they
were created.

Local variable: Here, car_list is a local variable within the print_cars() function. Printing car_list[0] at the end will
not work here because it is not available outside the print_cars() function.

```python
    def print_cars():
        car_list = ["Cadillac", "Toyota", "Ford"]
        for car in car_list:
            print(f"My car is a {car}.")

    print_cars()
    print(car_list[0])
```

Global variable: Here, car_list is a global variable, defined outside the scope of any function. It can be referenced both inside
and outside the function call.

```python
    car_list = ["Cadillac", "Toyota", "Ford"]

    def print_cars(car_list):
        for car in car_list:
            print(f"My car is a {car}")
    
    print_cars(car_list)
    print(car_list[0])

```

#### How do the global and nonlocal keywords work in Python, and in what situations might you use them?

The global keyword allows you to assign values to global variables within
a function. The normal behavior would be to assign that value to a new,
local variable with the same name as the global variable, but by using the
globa keyword, you can specify that you are reassigning the new value to
the global variable instead.

The nonlocal keyword acts much the same way as the global keyword, but is
used when you're referring to a variable in an enclosing scope, rather than
a truly global variable. This is helpful for being specific about which
variable you are referring to when using nested functions, for example.

#### In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis

Big O notation helps us identify how efficient our proposed solutions are
likely to be. Often times, the examples we use are very simple in nature.
While a proposed solution may work very fast in these examples, understanding
how they will scale is extremely important once those solutions are used in
real-world examples. Big O notation helps us understand why a solution might
not work well if it's repeated 5 million times or 1 billion times if it takes
too long or uses a tremendous amount of memory.

#### Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials

You would simulate a dice roll in Python by using the randint function with limits of
1 and 6. The resulting integer would be a dice roll. By repeating this process in a for
loop, you could then keep track of the total frequency of each number occurring in dice
rolls over a large number of trials. Over a large number, you could then divide the
frequency of each result by the total number of rolls to determine the approximate
probability of rolling any particular die, which would be about 1/6.
