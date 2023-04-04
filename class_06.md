# Class 06

**Date Due:** April 4, 6:30 pm PDT

## Reading

- [_How to Use Random Module_](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
- [_What is Risk Analysis_](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
- [_Test Coverage_](https://martinfowler.com/bliki/TestCoverage.html)

## Video

- [_Big O Notation_](https://www.youtube.com/watch?v=v4cd1O4zkGw)

### Reading Questions

#### How can the random module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module?

The random module can be used to create a random selection in a variety of ways. Whenever a
random number or random selection from a collection of items is needed in a program, the
random module has ways of producing the desired result. These can be particularly useful in
games (such as simulating the roll of a pair of dice) or can produce random-appearing input,
or any of a variety of other uses.

##### Common functions

- randint(start, stop) produces a random number within a range between start and stop (both inclusive)
- random() produces a floating point number between 0 and 1
- choice([options]) will select a random choice from the options list.

#### In the context of software development, what is risk analysis, and what are the key steps involved in conducting a risk analysis for a software project?

Risk analysis is the process of looking for potential dangers related to your development project
and taking steps to ensure that they are mitigated as effectively as possible. This includes making
a determination of the severity of the various risk factors and assigning resources to eliminating
those risks accordingly.

The general steps involved include:

- Searching for the risk
- Analyzing the impact of each risk
- Identifying the measures appropriate to mitigating each risk

_Note:_ These steps are taken directly from the reading material _What is Risk Analysis_ linked above.

Understanding what risks are involved, judging their potential impact, and taking the steps to ensure
that the level of risk is acceptable requires a nuanced, teamwork-based approached, but this is a
necessary appropach to be successful in software development.

#### What is test coverage and why is it an important (or potentially misleading) metric in software testing?

Test coverage is a measure of how much of your project's code is covered by tests. Theoretically, a
higher number is a good indicator for your project, but it is often a misleading statistic. While
understanding this percentage-based figure can be important, it is critical to understand that it makes
absloutely no determination about the _quality_ of the testing involved. A project with 100% coverage,
when those tests are inadequate, can be far less valuable than a project that has been 80% covered by
tests that have been thoughtfully designed and are likely to develop real, important deficincies.

#### What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity

Big O notation describes how an algorithm effects the use of time or memory, given changing sizes of input.
When an process takes the same amount of time, regardless of the size of the input, that is said to be using
constant time, or O(1) time complexity. Similarly, a process whose memory requirements do not change with
the size of the input has O(1) space complexity.

When time or memory requirements increase at the same rate as the size of the input, that is said to have
linear, or O(n) time or space complexity. In computer science, this notation often refers to algorithms
where program iterates over each item in the input once. Iterating over 3 items takes roughly one-millionth
of the time that iterating over 3 million items does.

A real world example of O(n) time complexity would be like hanging out your clothes to dry. One item of clothing
would take only a few seconds, but that time increases as there are more items of clothes to hang out.
