# Class 19

**Date Due:** May 20, 9am PDT

## Reading

- [_Python Regular Expressions Tutorial_](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)
- [_shutil_](https://pymotw.com/3/shutil/)

## Video

- [_Automation Ideas_](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)

## Reading Questions

### How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary library to work with them?

Regular expressions can be used in Python to search for patterns but importing the re library. Using methods such as .match(), you build up
expression strings that represent patters that are being searched for. Patterns consist of regular characters, wildcard characters that can
represent any character, and special identifiers, such as ^ to represent the beginning of a string, $ to represent the end of the string,
and brackets to represent ranges of characters being searched for, for example, [0-9] would represent a search for any character between 0
and 9.

### What is the purpose of the shutil library in Python, and provide an example of a common use case for file or directory management with this library?

The shutil library allows for file operations, such as copying and archiving. One common use is for archiving files using the make_archive()
function, This allows you to take a number of files and incorporate them into one of the archive formats that are available on your system
(such as tar or zip).

### Explain one automation idea from the assigned material and describe how it can be implemented using Python’s regular expressions and shutil libraries

One of the automation ideas was a utility that monitored a folder and automatically moved and renamed files as soon as they appeared. One could
use regex to specify certain types of files, or filenames that match a specific pattern, to decide which files to perform operations on. In addition,
you could use the shutil library to perform the file operations, such as copying or achiving the files that match the specified pattern.
