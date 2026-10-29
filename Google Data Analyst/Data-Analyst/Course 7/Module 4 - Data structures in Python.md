* **Data structures:** Collections of data values or objects that contain different data types.
* **List:** A data structure that helps store and manipulate an ordered collection of items.
* **Sequence:** A positionally ordered collection of items.
* **Mutability:** The ability to change the internal state of a data structure.
* **Immutability:** A data structure or element's values can never be altered or updated.
* `append()`: Method that adds an element to the end of a list.
* **Tuple:** An immutable sequence that can contain elements of any data type.
* **List comprehension:** Formulaic creation of a new list based on the values in an existing list.
	* `my_list = [expression for element in iterable if condition]`
* `zip()`: A python function that performs an element-wise combination of sequences.
	* We can unzip with the \* operator like `zip(*scientists)`
* `enumerate()`: Allows you to iterate over a sequence while keeping track of each element's index.
* **Dictionary:** A data structure that consists of a collection of key-value pairs.
* `dict()`: Function used to create a dictionary.
* `del` keyword to delete a key-value pair from a dictionary.
* **Set:** A data structure in Python that contains only unordered, non-interchangeable elements.
* **Library(or package):** Broadly refers to a reusable collection of code.
* **Matplotlib:** A library for creating static, animated, and interactive visualizations in Python.
* **Seaborn:** A visualization library based on matplotlib that provides a simpler interface for working with common plots and graphs.
* **Numpy:** An essential library that contains multidimensional array and matrix data structures and functions to manipulate them.
* **Pandas:** A powerful llibrary built on top of numpy that's used to manipulate and analyze tabular data.
* **Module:** A simple python file containing a collection of functions and global variables.
* **Global variables:** Variables that can be accessed from anywhere in a program or script.
* **Vectorization:** Enables operations to be performed on multiple components of a data object at the same time.
* **N-dimensional array:** The core data object of numPy.
* `dtype:` A numpy attribute used to check the data type of the contents of an array.
* `shape:` A NumPy attribute used to check the shape of an array.
* `reshape():` NumPy method used to change the shape of an array.

### How NumPy arrays store data in memory

NumPy arrays work by allocating a contiguous block of memory at the time of instantiation. Most other structures in Python don’t do this; their data is scattered across the system’s memory. This is what makes NumPy arrays so fast; all the data is stored together at a particular address in the system’s memory. 

Interestingly, this is also what prevents an array from being lengthened or shortened: The abutting memory is occupied by other information. There’s no room for more data at that memory address. However, existing elements of the array can be replaced with new elements. 

![A diagram of system memory. A NumPy array sits directly in between other data structures. There’s no room to add values.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/pqhYWhaiSQyNyx07DdIX2w_1a2be9b965fb4838baf381328684d0f1_i18cUuYTfItYUj13cpSCIv9JTIRPFAMFG8A6fT_ez7vUuVPDcfnKPNJuaOhGgZRG2cESSaWgXJOFtREBJeCKtI_ZXCTwguxgpP6NXQMLK0druUIoqRUtdgPeiqDx_8N3ARwFwQ7k3kwtV5kNlKEiBIFSZKTee-eRj7dL0DctrqafP6-xCP83lrCmTIklFhSisSxGTCkp15rzvXq78OIO1abeI7kmAT5IXlVBMQ?expiry=1786903817154&hmac=sNqo26ytnH9w5YpuU4BK6s_wWTO0eS4Lj4-bP4skGLI)

The only way to lengthen an array is to copy the existing array to a new memory address along with the new data.

## Pandas
* **Tabular data:** Data that is in the form of a table, with rows and columns.
* **DataFrame:** A two-dimensional, labeled data structure with rows and columns.
* **CSV file:** Stands for "comma-separated values." A plaintext file that uses commas to separate distinct values from one another.
* **Series:** A one-dimensional, labeled array.
* `iloc[]`: A way to indicate in pandas that you want to select by integer-location-based position.
* `loc[]`: Used to select pandas rows and columns by name


### **Primary data structures**

Pandas has two primary data structures: Series and DataFrame. 

- **Series**: A Series is a one-dimensional labeled array that can hold any data type. It’s similar to a column in a spreadsheet or a one-dimensional NumPy array. Each element in a series has an associated label called an index. The index allows for more efficient and intuitive data manipulation by making it easier to reference specific elements of your data.
    
- **DataFrame**: A dataframe is a two-dimensional labeled data structure—essentially a table or spreadsheet—where each column and row is represented by a Series.

* **Boolean Masking:** A filtering technique that overlays a Boolean grid onto a dataframe in order to select only the values in the dataframe that align with the True values of the grid.
* `groupby()`: A pandas DataFrame method that groups rows of the dataframe together based on their values at one or more columns, which allows further analysis of the groups.
* `agg()`: Short for "aggregate". A pandas groupby method that allows you to apply multiple calculations to groups of data.

## groupby()

The [groupby()](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html) function is a method that belongs to the DataFrame class. It works by splitting data into groups based on specified criteria, applying a function to each group independently, then combining the results into a data structure. When applied to a dataframe, the function returns a groupby object. This groupby object serves as the foundation for different data manipulation operations, including:

- Aggregation: Computing summary statistics for each group
    
- Transformation: Applying functions to each group and returning modified data
    
- Filtration: Selecting specific groups based on certain conditions
    
- Iteration: Iterating over groups or values

### Built-in aggregation functions

The previous examples demonstrated the mean(), min(), and size() aggregation functions applied to groupby objects. There are many available built-in aggregation functions. Some of the more commonly used include:

- count(): The number of non-null values in each group
    
- sum(): The sum of values in each group
    
- mean(): The mean of values in each group
    
- median(): The median of values in each group
    
- min(): The minimum value in each group
    
- max(): The maximum value in each group
    
- std(): The standard deviation of values in each group
    
- var(): The variance of values in each group

## **MultiIndex**

You might have noticed that, when functions are applied to a groupby object, the resulting dataframe has tiered indices. This is an example of **MultiIndex**. MultiIndex is a hierarchical system of dataframe indexing. It enables you to store and manipulate data with any number of dimensions in lower dimensional data structures such as series and dataframes. This facilitates complex data manipulation.


* `concat()`: A pandas function that combines data either by adding it horizontally as new columns for existing rows, or vertically as new rows for existing columns.
* `merge()`: A pandas function that joins two dataframes together; it only combines data by extending along axis one horizontally.
* **Keys:** The shared points of reference between different dataframes - what to match on


# Terms and definitions from Course 7, Module 4

**agg()**: A pandas groupby method that allows the user to apply multiple calculations to groups of data

**Aliasing**: A process that allows the user to assign an alternate name—or alias—to something

**append()**: A method that adds an element to the end of a list

**Boolean masking**: A filtering technique that overlays a Boolean grid onto a dataframe in order to select only the values in the dataframe that align with the True values of the grid

**concat()**: A pandas function that combines data either by adding it horizontally as new columns for existing rows or vertically as new rows for existing columns

**CSV file**: A plaintext file that uses commas to separate distinct values from one another; Stands for "comma-separated values”

**Data structure**: A collection of data values or objects that contain different data types

**DataFrame**: A two-dimensional, labeled data structure with rows and columns

**dict()**: A function used to create a dictionary

**Dictionary**: A data structure that consists of a collection of key-value pairs

**difference()**: A function that finds the elements present in one set but not the other

**dtype**: A NumPy attribute used to check the data type of the contents of an array

**Global variable**: A variable that can be accessed from anywhere in a program or script

**groupby()**: A pandas DataFrame method that groups rows of the dataframe together based on their values at one or more columns, which allows further analysis of the groups

**iloc[]**: A type of notation in pandas that indicates when the user wants to select by integer-location-based position

**Immutability**: The concept that a data structure or element’s values can never be altered or updated

**Import statement**: A statement that uses the import keyword to load an external library, package, module, or function into the computing environment

**Inner join**: A way of combining data such that only the keys that are in both dataframes get included in the merge

**insert()**: A function that takes an index as the first parameter and an element as the second parameter, then inserts the element into a list at the given index

**intersection()**: A function that finds the elements that two sets have in common

**items()**: A dictionary method to retrieve both the dictionary’s keys and values

**Keys**: The shared points of reference between different dataframes

**keys()**: A dictionary method to retrieve only the dictionary’s keys

**Left join**: A way of combining data such that all of the keys in the left dataframe are included, even if they aren’t in the right dataframe

**Library**: A reusable collection of code; also referred to as a “package”

**List**: A data structure that helps store and manipulate an ordered collection of items

**List comprehension**: Formulaic creation of a new list based on the values in an existing list

**loc[]**: Notation that is used to select pandas rows and columns by name

**matplotlib**: A library for creating static, animated, and interactive visualizations in Python

**merge()**: A pandas function that joins two dataframes together; it only combines data by extending along axis one horizontally

**Module**: A simple Python file containing a collection of functions and global variables 

**Mutability**: The ability to change the internal state of a data structure

**N-dimensional array**: The core data object of NumPy; also referred to as “ndarray”

**NaN**: How null values are represented in pandas; stands for “not a number”

**ndim**: A NumPy attribute used to check the number of dimensions of an array

**Nested loop**: A loop inside of another loop

**NumPy**: An essential library that contains multidimensional array and matrix data structures and functions to manipulate them

**Outer join**: A way of combining data such that all of the keys from both dataframes get included in the merge

**pandas**: A powerful library built on top of NumPy that’s used to manipulate and analyze tabular data

**pop()**: A method that extracts an element from a list by removing it at a given index

**remove()**: A method that removes an element from a list

**reshape()**: A NumPy method used to change the shape of an array

**Right join**: A way of combining data such that all the keys in the right dataframe are included—even if they aren’t in the left dataframe

**Seaborn**: A visualization library based on matplotlib that provides a simpler interface for working with common plots and graphs

**Sequence**: A positionally ordered collection of items

**Series**: A one-dimensional, labeled array where the data type must be the same for all the data in a given series

**Set**: A data structure in Python that contains only unordered, non-interchangeable elements

**set()**: A function that takes an iterable as an argument and returns a new set object

**shape**: A NumPy attribute used to check the shape of an array

**symmetric_difference()**: A function that finds elements from both sets that are mutually not present in the other

**Tabular data**: Data that is in the form of a table, with rows and columns 

**Tuple**: An immutable sequence that can contain elements of any data type

**tuple()**: A function that transforms input into tuples

**type()**: A function used to identify the type of data in a list

**union()**: A function that finds all the elements from both sets

**values()**: A dictionary method to retrieve only the dictionary’s values

**Vectorization**: A process that enables operations to be performed on multiple components of a data object at the same time