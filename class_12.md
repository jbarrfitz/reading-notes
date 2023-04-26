# Class 12

**Date Due:** April 25, 6:30 pm PDT

## Reading

- [_Pandas in 10_](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)
- [_Pandas - Getting Started_](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)
- [_Corey Schafer - Pandas Tutorials_](https://www.youtube.com/playlist?list=PL-osiE80TeTsWmV9i9c58mdDCSskIFdDS)

## Video

- [_What is Pandas_](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)

## Bookmark and Reivew

- [_Master Pandas_](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)

### Reading Questions

#### Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?

Pandas takes large sets of data and converts them into DataFrames, which essentially act like spreadsheets or data tables and allows
you to manipulate them. You can perform common data operations on them, such as finding sums, min, max, mean, mode, etc., as well as
filter, sort, group, and perform aggregate functions. Since it is so performant, it allows you to easily perform these operations on
very large sets of data.

#### What are the primary data structures in Pandas, and how do they differ in terms of use cases?

Series are one-dimensional and essentially represent one column of information, whereas DataFrames are collections of Series that
comprise an entire table. Series are generally used to analyze a single point of data among many records, and DataFrames allows you
to compare and contrasts many different points of data among many records.

#### Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?

Esssentially you create a DataFrame by importing Pandas into your project and then read the data in any of the many supported formats,
including:

- CSV: pd.read_csv('file_path')
- Excel: pd.read_excel('file_path')
- JSON: pd.read_json('file_path')
- SQL: pd.read_sql('SELECT * FROM table', connection)
