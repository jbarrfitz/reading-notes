# Class 01

**Date Due:** March 21, 6:30pm PDT

## Reading

- _In Tests We Trust - TDD with Python_
- _If name equals main_
- _Recursion_

## Video

- _What on Earth is Recursion_

### Notes

#### In Tests We Trust

Test-driven development is an approach to development in which the developer writes tests
firsts and then develops code designed to pass those tests. By searching for things that
_can_ go wrong, it enables the developer to think more carefully about edge cases and other
problems that can present themselves when algorithms are not thoroughly examined for their
effects. This approach can lead to cleaner code and less debugging later in the process.

**What I would like to know more about:** How TDD is really used in the business world. It
has been my experience in speaking with working developers that there are many companies that
"talk the talk" of TDD, but few actually "walk the walk."

#### If name equals main

The standard line of code:

```python
if __name__ = "__main__"
```

is an easy way to determine whether a Python module is running from the top level or if it
is being called by another module. Since dunder-name is always defined, this quick check allows
you to control what code is being run, depending on its context.

#### Recursion

Recursion is the process of creating a function that calls itself. This can be a useful shorthand
tool for lots of repetitive functions, for example, calculating a fibonacci sequence. There is a
steep learning curve, however, and the pitfalls of creating a recursive function include the ease
with which one can create a function that loops endlessly.

Special attention needs to be made to creating appropriate end tests when using recursive functions,
but when done correctly, they can save a lot of extra coding.

**What I would like to know more about:**
Recursion is a tricky skill to learn, and frankly it's one that I avoid unless a problem very clearly
calls for its use. Wrapping my head around how they work is a skill I need to improve upon.
