# Class 03

**Date Due:** March 25, 9 am PDT

## Reading

- [_Read and Write Files in Python_](https://realpython.com/read-write-files-python/)
- [_Exceptions in Python_](https://realpython.com/python-exceptions/)

## Video

- [_Read and Write Files in Python - Companion Video_](https://realpython.com/courses/reading-and-writing-files-python/)

### Summary

The ability to read and write files is a key feature of Python, as it enables the
developer to use input from a variety of sources that provides context to the application
being written.

### Notes

#### Read and Write Files in Python

Python has a number of built-in functions that allow for the reading and writing of various
types of files. These files may be created for the purposes of output, e.g., an application where
the user might have the ability to download a file that has been custom-created based on selections
they have made in the application; or it may be for reading purposes, e.g., an application that takes
files that have been generated by a third-party application which are then used as input by our new
app.

Best practice when dealing with files is to always close once the program has finished any operations,
which is important because of potential security leaks (open files may be accessible to other resources),
and for resource management purposes, since closing the file will free up the space used for that resource.

#### Exceptions in Python

There are few methods for handling exceptions in Python, most commonly the Try-Except-Else-Finally block. With
these blocks, the code that could potentially fail is found within the Try clause. The Except clause contains
the code describing how to handle that failure. Best practices here include specifying as much as possible
the types of errors you would expect to see in this block, since failing to do so enables to the program to
handle **all** errors, including ones you don't necessarily want handled. In the Else block lies the code
that is meant to execute if no exceptions are found. In the Finally clause, you would include code that needs
to run regardless of whether an exception was raised, which generally involves any cleanup of the code.

## What I would like to know more about

- What are the best ways of handling exceptions in cases where the exception indicates that there is no access to a resource that you would reasonably need to continue?
