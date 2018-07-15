---
title: "Reading Spreadsheet Data into Pandas DataFrames"
teaching: 10
exercises: 10
questions:
- "How can I read my spreadsheet data into Python?"
- "What is Pandas and how do I use it?"
- "How can I inspect my data in Pandas Python?"
objectives:
- "Import the Pandas library."
- "Use Pandas to load a simple CSV data set."
- "Produce basic information about a Pandas Data Frame."
keypoints:
- "Use the Pandas library to get basic statistics information about tabular data."
- "Use `index_col` to specify that a column's values should be used as row headings."
- "Use `DataFrame.info` to find out more about a dataframe."
- "The `DataFrame.columns` variable stores information about the dataframe's columns."
- "Use `DataFrame.T` to transpose a dataframe."
- "Use `DataFrame.describe` to get summary statistics about data."
---
## Use the Pandas library to do statistics on tabular data.

*   Pandas is a widely-used Python library for statistics, particularly on tabular data.
*   Borrows many features from R's Data Frames.
    *   A 2-dimensional table whose columns have names
        and potentially have different data types.
*   Load it with `import pandas`.
*   Read a Comma Separate Values (CSV) data file with `pandas.read_csv`.
    *   Argument is the name of the file to be read.
    *   Assign result to a variable to store the data that was read.

~~~
import pandas

data = pandas.read_csv('data/some-lib-data.csv')
print(data)
~~~
{: .python}
~~~
