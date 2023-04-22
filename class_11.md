# Class 11

**Date Due:** April 22, 9 am PDT

## Reading

- [_What is Jupyter Lab_](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)
- [_Numpy Tutorial_](https://www.dataquest.io/blog/numpy-tutorial-python/)

## Bookmark and Reivew

- [_Numpy Arrays_](https://www.tutorialspoint.com/numpy/index.htm)

### Reading Questions

#### What are the key features and benefits of Jupyter Lab, and how does it differ from Jupyter Notebook?

Jupyter Lab is essentially the web-based implementation of Jupyter notebooks. It allows for working with
many, many different file formats and uses a series of keyboard shortcuts optimized for use on a web-based
platform to perform common operations. It's a powerful tool that combines the power of custom components
such as terminals and text editors to create powerful notebooks with multiple tabs and splits and a unified
workflow for your projects.

#### What are the main functionalities provided by the NumPy library, and how can it be useful in Python programming, particularly for scientific computing and data manipulation tasks?

NumPy allows for working with arrays of varying numbers of dimensions. It's very powerful for performing the
same operations on many different elements within an array, and for performing calculations and combinations
between multiple arrays. These features allow for the very quick computation of multiple, large datasets,
which is particularly useful for scientific computing and data maniuplation tasks.

#### Explain the basic structure and properties of NumPy arrays, and provide examples of how to create, manipulate, and perform operations on them

The basic structure of a NumPy array is similar to nested lists within Python. For example, a two-dimensional
array would be represented as:

```python
[
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
]
```

Some of the more common properties of NumPy arrays include:

- shape: the size of the array in each of the dimensions. In the example above, the size is (3, 3) since it has 3 rows and 3 columns
- size: a total count of elements in the array. In the example, this would be 9
- ndim: the number of dimensions in the array. There are 2 in the example
- dtype: the dtype of the example array is int64 (64-bit integer)

NumPy arrays can be created by passing them in as tuples or lists (or other iterables) into the array method of numpy, for example:

```python
arr = np.array([1, 2, 3, 4])
```

You can also perform maxtrix operations on them, such as adding their individual values:

```python
arr = np.array([1, 2, 3])
arr1 = np.array([4, 5, 6])
arr2 = arr + arr2 # [5, 7, 9]
```

You can perform operations on NumPy arrays to manipulate them, such as concatenation:

```python
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
arr3 = np.concatenate(arr1, arr2) # [1, 2, 3, 4, 5, 6]
```

Or transposing them (flipping them on their axes):

```python
arr1 = np.array([[1, 2], [3, 4]])
arr2 = np.transpose(arr1) # [[1, 3], [2, 4]]
```
