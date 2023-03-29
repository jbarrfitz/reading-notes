# Class 04

**Date Due:** March 28, 6:30 pm PDT

## Reading

- [_Classes and Objects_](https://www.learnpython.org/en/Classes_and_Objects)
- [_Thinking Recursively_](https://realpython.com/python-thinking-recursively/)
- [_Pytest Fixtures and Coverage_](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

### Summary

Classes and objects (or object-oriented programming in general) is one of the most important concept to understand for
an aspiring developer, as it is a concept that is used constantly throughout software engineering. The ability to model
real-world circumstances through these tools is a powerful concept that must be thoroughly understood in order to be
successful.

Recursive functions are commonly-used tools to solve problems without having to write a lot of repetitive code, and
they can often be easier to understand once written (although they can be a bit more difficult to conceptualize). It
is a tool that can aid in making more powerful and more comprehensible code.

The article on pytest fixtures and coverage has helped to expand my knowledge of testing procedures, as it offers two
more concepts that will definitely be helpful in making sure that tests are written more effectively, and that those
tests are covering every area of need within a given program.

### Review Questions

- What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

Classes are the "templates" from which objects are created. One first builds a class and decides what methods and variables should belong
to all items belonging to that class. Once that has been achieved, you create an "instance" of that class, known as an object. "Car" might
be a class, but "JerrysCar" would be akin to the object, it is a specific "Car" that has specific data associated with it, such as its
make, model, year, owner, color, etc.

- Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

Recursion is a function that calls itself. In other words, a function will rely on the result of a previous iteration of that function in order to
calculate the new result. The classic example of this is calculating factorials:

- 1! = 1
- 2! = 2 x 1
- 3! = 3 x 2 x 1
- 4! = 4 x 2 x 1

To put it more succinctly . . .

- 1! = 1
- 2! = 2 x 1!
- 3! = 3 x 2!
- 4! = 4 x 3!

So the easiest way to calculate 4! is by multiplying 4 and 3!, which is calculated by multiplying 3 and 2! . . . this process is repeated until
you get down to 1, at which point you can just return the number one. Each instance of calling the recursive factorial function merely calls on the
result of the previous iteration.

Best practices for recursive functions include making sure that you have a correct base case, which is the point at which your recursive function
should stop calculating. Failing to do this will likely send the program into an endless loop or cause some other type of error, such as dividing
by zero.

- What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.

Pytest fixtures are an easy way to reuse the same functions throughout the testing suite. This makes tests easier to write and cleaner to understand.
It avoids repetitive code, since you won't have to write that same code over and over again. Writing effective tests using fixtues can also be paired
with generating coverage reports via pytest-cov, which help point out if there are any areas of the code that lack testing coverage.

#### Classes and Objects

Classes and objects are at the heart of any object-oriented language, such as Python. The ability to take "templates"
(classes) and create instances of those classes (objects) is critical to modeling real-world problems and being able
to solve those issues. Any class can have its own variables (properties) and methods (functions), and every object
created from that class has access to those properties and methods. Accessing these items from an existing class,
or assigning values to those, requires only simple dot notation in python, e.g., object1.property

#### Thinking Recurseively

Recurive algorithms are at the heart of a lot of programming issues, particularly ones where the same operation needs
to be repeated over a collection of data, such as a list, set, or dictionary. When solving a problem requires the
reptition of a process, and that repetition can be made faster by using the data from previous processes from the set,
a strong case for recursion exists. There are a couple of methods for keeping track of the current state of a recursive
function, including maintaining a global variable that tracks the current state, or by designing a recursive function
that explicitly relies on the result of the previous iteration of that function, although in the author's opinion,
the latter method is preferrable to the former. Practice with recursive functions is required, as it allows one to
more effectively write base and recursive cases for these functions and effectively utilize the stack.

#### Pytest Fixtures and Coverage

The pytest testing suite allows for a number of options when testing for the effectiveness and accuracy of your code. Fixtures
are functions that act like global variables, in that they can be called throughout the testing suite, rather than being accessed
by only one particular test. This simplifies writing tests, as you can access the same functions again and again rather than
re-writing.

The pytest-cov is a powerful tool that can be used to determine how much of a program is being covered by testing. While a score of
100% does not indicate that a program has without errors, it does indicate that all areas of the program have been tested in _some_
way. Rather than indicating a perfect series of tests, it is most helpful in that it indicates deficiencies in testing, such as
functions within a program that have not been tested at all. Coverage reports can be written to a variety of formats, although HTML
is the most common and likely the easiest.

## What I would like to know more about

- I do not have a lot of experience with testing, so I really need to go much more in-depth about which tests are the most effective and appropriate for any given situation.
- The article about fixtures did a good job of introducing the concept, but without the accompanying knowledge of testing procedures, it is hard to see exactly how they will be useful and under what circumstances.
