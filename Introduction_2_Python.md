# Introduction to Python
Python is a high-level, interpreted, and general-purpose programming language. It was created by Guido van Rossum and first released in 1991. Python is known for its simplicity, readability, and versatility, making it a popular choice for various applications, including web development, data science, artificial intelligence, automation, and scientific computing.

## Introducing Variables
In any programming language, variables are used to store and manipulate data. A variable is essentially a named storage location in a computer's memory where a programmer can store data, and its value can be changed during the execution of a program. Variables have a specific data type, such as integer, floating-point, character, etc., which defines the kind of data they can hold.

The assignment operator (=) is used to assign a value to a variable. The syntax is typically as follows:


```python
# x is a variable. '=' is used to assign the value 10 to variable x.
x=10;
print(x);
```

    10


It is very important to remember what name you are giving each variable . Python has some reserved keywords which cannot be used to name any variable : e.g. def, class, global, if, in, etc.

## Data Types in Python
Python has several built-in data types that are used to represent different kinds of data. Here are some of the fundamental data types in Python:

* Numeric Types:

-int: Integer type, e.g., 10, -3, 42.\
-float: Floating-point type, e.g., 3.14, -0.5, 2.0.

* Sequence Types:

-str: String type, e.g., "Hello, World!", 'Python'.\
-list: List type, ordered and mutable sequence, e.g., [1, 2, 3], ['apple', 'banana'].\
-tuple: Tuple type, ordered and immutable sequence, e.g., (1, 2, 3), ('a', 'b').

* Set Types:

-set: Unordered collection of unique elements, e.g., {1, 2, 3}, {'apple', 'orange'}.

* Mapping Type:

-dict: Dictionary type, a collection of key-value pairs, e.g., {'name': 'John', 'age': 25}.

* Boolean Type:

-bool: Boolean type, representing True or False.
* None Type:

-NoneType: The type of the None object, representing the absence of a value.

### Numeric DataType
In Python, numeric data types are used to represent numerical values. The primary numeric data types in Python are: \

* int (Integer): Integer data type represents whole numbers without any decimal points. ​

* float (Floating-Point): Float data type represents numbers with decimal points or exponential notation.​

* complex (Complex Numbers): Complex data type represents numbers in the form of a real part and an imaginary part. Complex numbers are written as a + bj, where a is the real part, b is the imaginary part, and j is the imaginary unit.


```python
#Numeric data type
x = 10
type(x)
```




    int




```python
y = 2.34
type(y)
```




    float




```python
z = 2 + 3j
type(z)
```




    complex




```python
#Arithmatic operations on Numeric datatypes
addition = x+y+z
print("Sum of x,y,z is ",addition)

product= x*y
print("Product is ",product)
```

    Sum of x,y,z is  (14.34+3j)
    Product is  23.4


### Sequence Data Type
Sequence data types in Python are collections of ordered and indexed elements. These elements can be of different data types, and the sequence maintains the order in which they are inserted. Here are some of the main sequence data types in Python: 

Lists: 

* Lists are ordered and mutable sequences.​

* Elements can be of different data types.​

* Lists are defined using square brackets [].​

Tuples:​

* Tuples are ordered and immutable sequences.​

* Elements can be of different data types.​

* Tuples are defined using parentheses ()​

Strings:​

* Strings are ordered sequences of characters.​

* Strings are immutable in Python.​

* Strings are defined using single (') or double (") quotes.​




```python
#Sequence Data Type
my_list = [1, 2, 'apple', 3.14, True] #this is a list character
my_tuple = (1, 2, 'banana', 3.14, False)
my_string = "Hello, Python!"
my_range = range(5)  # Represents the numbers 0, 1, 2, 3, 4
print("The list is {} , the tuple is {} and string is {}.".format(my_list,my_tuple,my_string))
```

    The list is [1, 2, 'apple', 3.14, True] , the tuple is (1, 2, 'banana', 3.14, False) and string is Hello, Python!.



```python
#Slicing and Indexing elements from a list

abc=[12,13,14,15,16,17,18,19,20,22,28,29,32,24,25,32,35];
print(abc[0]);
print(abc[2]);
print(abc[1:7]) #start index: end index -1th index
print(abc[:7]) #0th index : 7-1th index
print(abc[2:])
print(abc[-1])
print(abc[-2])
```

    12
    14
    [13, 14, 15, 16, 17, 18]
    [12, 13, 14, 15, 16, 17, 18]
    [14, 15, 16, 17, 18, 19, 20, 22, 28, 29, 32, 24, 25, 32, 35]
    35
    32



```python
#nested_lists

pqr=[12,13,[25,26,27],14,16,17,[44,46,[76,77,78],48],19];
print(pqr[1]);
print(pqr[2][1]);
print(pqr[6][1]);
print(pqr[6][2][2])
```

    13
    26
    46
    78


### Set DataType
In Python, a set is a built-in data type that represents an unordered collection of unique elements. Sets are useful for various operations, such as testing membership, removing duplicates from a sequence, and performing set operations like union, intersection, and difference.Sets are particularly useful when you need to work with unique elements, and they offer efficient methods for performing set operations. Additionally, sets are mutable, allowing you to modify their contents after creation.


```python
#Set Data Type
# Using curly braces
my_set = {1, 2, 3, 4, 5}

# Using set() constructor
another_set = set([2, 4, 6, 8, 10])
print(my_set)
print(another_set)
```

    {1, 2, 3, 4, 5}
    {2, 4, 6, 8, 10}



```python
#Adding and Removing Elements:

#You can add elements to a set using the add() method.
#Elements can be removed using the remove() or discard() methods.
my_set.add(6)
my_set.remove(3)
print(my_set)
```

    {1, 2, 4, 5, 6}



```python
#Operations on Sets:

#Union (|): Combines elements from two sets.
#Intersection (&): Retrieves common elements between two sets.
#Difference (-): Retrieves elements in the first set but not in the second.
#Symmetric Difference (^): Retrieves elements in either set, but not both.
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

union_result = set1 | set2
intersection_result = set1 & set2
difference_result = set1 - set2
symmetric_difference_result = set1 ^ set2

print(union_result)
print(intersection_result)
print(difference_result)
print(symmetric_difference_result)
```

    {1, 2, 3, 4, 5, 6}
    {3, 4}
    {1, 2}
    {1, 2, 5, 6}



```python
#Membership Test:

#You can check if an element is present in a set using the in keyword.
print(2 in my_set) 
print(7 in my_set) 

```

    True
    False



```python
#Set Methods:
#Sets have various methods for performing operations and manipulations, 
#such as pop(), clear(), copy(), and update().
my_set.pop()        # Removes and returns an arbitrary element
print(my_set)
```

    {2, 3, 4, 5}



```python
set_copy = my_set.copy()  # Creates a shallow copy of the set
print(set_copy)
```

    {2, 3, 4, 5}



```python
my_set.clear()      # Removes all elements from the set
print(my_set)
```

    set()


### Mapping DataType

In Python, the built-in mapping data type is called a dictionary. A dictionary is an unordered collection of key-value pairs, where each key must be unique. Dictionaries are also known as associative arrays or hash maps in other programming languages


```python
#Creating a Dictionary:
#You can create a dictionary using curly braces {} and specifying key-value pairs using colons ':'.
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
print(my_dict)
```

    {'name': 'John', 'age': 25, 'city': 'New York'}



```python
#Accessing Values:
#You can access the values in a dictionary using the keys.
print(my_dict['name'])  # Output: John

```

    John



```python
#Adding and Modifying Elements:
#You can add new key-value pairs or modify existing ones.
my_dict['occupation'] = 'Engineer'
my_dict['age'] = 26
print(my_dict)
```

    {'name': 'John', 'age': 26, 'city': 'New York', 'occupation': 'Engineer'}



```python
#Removing Elements:
#You can remove a key-value pair using the pop() method or the del statement.
my_dict.pop('age')
# or
del my_dict['name']
print(my_dict)
```

    {'city': 'New York', 'occupation': 'Engineer'}


### Boolean and None Data Types

Both the boolean data type and the NoneType are fundamental in Python, and understanding their usage is crucial for writing effective and correct code. Booleans are commonly used in logical and conditional statements, while None is often used to represent the absence of a value or to initialize variables.

~ Boolean Data Type (bool):

The bool data type represents boolean values, either True or False.
Boolean values are often used for making decisions in control flow statements, such as if statements.
Boolean values can result from comparison operations, logical operations, and other boolean expressions.



```python
# boolean data type
x = True
y = False

result = x and y  # Logical AND
print(result)

#In addition to True and False, 
#boolean values can also be the result of various expressions, 
#such as comparisons (<, >, ==, etc.) or logical operations (and, or, not).
```

~None Type (NoneType):

The NoneType has a single value, None, which represents the absence of a value or a null value.
It is often used to signify that a variable or a function does not have a meaningful result or to initialize a variable before assigning a real value.

## Basic Operations

Basic operations in Python cover a wide range of tasks, from arithmetic and logical operations to string manipulations. Here are some fundamental operations you can perform in Python:


```python
##Arithmatic Operations

# Addition
result_addition = 5 + 3
print(result_addition)

# Subtraction
result_subtraction = 7 - 2
print(result_subtraction)

# Multiplication
result_multiplication = 4 * 6
print(result_multiplication)

# Division
result_division = 10 / 2
print(result_division)

# Floor Division (returns the integer part of the division)
result_floor_division = 17 // 3
print(result_floor_division)

# Modulus (returns the remainder of the division)
result_modulus = 17 % 3
print(result_modulus)

# Exponentiation
result_exponentiation = 2 ** 4
print(result_exponentiation)
```

    8
    5
    24
    5.0
    5
    2
    16



```python
##Comparison Operations

# Equality
result_equal = 5 == 5

# Inequality
result_not_equal = 7 != 3

# Greater than
result_greater_than = 10 > 8

# Less than
result_less_than = 3 < 9

# Greater than or equal to
result_greater_equal = 5 >= 5

# Less than or equal to
result_less_equal = 4 <= 6

```


```python
##Logical Operations
# Logical AND
result_logical_and = True and False
print(result_logical_and)

# Logical OR
result_logical_or = True or False
print(result_logical_or)

# Logical NOT
result_logical_not = not True
print(result_logical_not)
```

    False
    True
    False



```python
## String Operations
# Concatenation
result_concatenation = "Hello, " + "World!"
print(result_concatenation)

# Repetition
result_repetition = "Python" * 3
print(result_repetition)

# String Length
string_length = len("Hello")
print(string_length)

# Indexing
first_char = "Python"[0]  # Accessing the first character
print(first_char)

# Slicing
substring = "Python"[1:4]  # Extracting a substring
print(substring)
```

    Hello, World!
    PythonPythonPython
    5
    P
    yth



```python
##List Operations
# Creating a list
my_list = [1, 2, 3, 4, 5]
print(my_list)

# Appending an element
my_list.append(6)
print(my_list)

# Removing an element
my_list.remove(3)
print(my_list)

# List Length
list_length = len(my_list)
print(list_length)

# Indexing
first_element = my_list[0]
print(first_element)

# Slicing
sublist = my_list[1:4]
print(sublist)
```

    [1, 2, 3, 4, 5]
    [1, 2, 3, 4, 5, 6]
    [1, 2, 4, 5, 6]
    5
    1
    [2, 4, 5]



```python
##Type Conversion 
# Integer to String
int_to_str = str(42)
print(int_to_str)
print(type(int_to_str))

# String to Integer
str_to_int = int("123")
print(str_to_int)

# Float to Integer
float_to_int = int(3.14)
print(float_to_int)

# Integer to Float
int_to_float = float(7)
print(int_to_float)
```

    42
    <class 'str'>
    123
    3
    7.0


## Controlled Structures 
In programming, control structures are used to manage the flow of a program by making decisions and repeating actions based on conditions. There are three main types of control structures: sequential, selection (conditional), and iteration (repetition). Let's explore each of them:

1. Sequential Structure:\
In a sequential structure, statements are executed one after another in a linear fashion. It is the default behavior of most programming languages.
2. Selection (Conditional) Structure:\
Selection structures allow the program to make decisions based on conditions. The most common form is the if statement.
3. Iteration (Repetition) Structure:\
Iteration structures allow the program to repeat a block of code multiple times. The most common forms are for and while loops.

In addition to these basic structures, Python also supports more advanced constructs like break and continue statements within loops, allowing for more fine-grained control over the flow of the program.


```python
# Sequential structure
statement1 = "This is the first statement."
statement2 = "This is the second statement."

print(statement1)
print(statement2)

```

    This is the first statement.
    This is the second statement.



```python
# Simple if statement
x = 10

if x > 0:
    print("x is positive.")

```

    x is positive.



```python
# If-else statement
y = -5

if y > 0:
    print("y is positive.")
else:
    print("y is non-positive.")

```

    y is non-positive.



```python
# If-elif-else statement
z = 0

if z > 0:
    print("z is positive.")
elif z < 0:
    print("z is negative.")
else:
    print("z is zero.")

```

    z is zero.



```python
# For loop
for i in range(5):
    print(i)

```

    0
    1
    2
    3
    4



```python
# While loop
counter = 0

while counter < 5:
    print(counter)
    counter += 1

```

    0
    1
    2
    3
    4


## Modules in Python
A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py added. Modules allow you to logically organize your Python code by grouping related functionality into separate files.

## os Module

The os module in Python provides a way of interacting with the operating system. It offers a range of functions to perform operations on the file system, handle paths, and execute system commands. Here are some commonly used features of the os module:


```python
#Get the Current Working Directory:
import os

current_directory = os.getcwd()
print(current_directory)


```

    /home/mediomix/Desktop/BioPython_Module



```python
#Change Directory 
#os.chdir('/path/to/new/directory')
#for e.g. : os.chdir('/home/mediomix/Desktop/')
os.chdir('/home/mediomix/Desktop/BioPython_Module/')
print(os.getcwd())
```

    /home/mediomix/Desktop/BioPython_Module



```python
#list_files_in_a_Directory
files_and_directories = os.listdir()  # in current directory what files are there
print(files_and_directories)

files_Desktop = os.listdir('/home/mediomix/Desktop/')
print(files_Desktop)
```

    ['Class 4.ipynb', 'Day 10.ipynb', 'Day 8.ipynb', 'Day 9.ipynb', 'Day1.ipynb', 'Day 6.ipynb', 'Day 11.ipynb', 'Day 5.ipynb', 'Day3.ipynb', 'Introduction_2_Python.ipynb', 'Day 12.ipynb', 'Day 7.ipynb', 'iris.csv', 'Day2.ipynb', '.ipynb_checkpoints']
    ['OmicsBox.desktop', 'Blast2GO.desktop', 'mag', 'cnvtrial1', 'ezTree', 'Sample_Metagenome_data-20230619T041709Z-001.zip', 'WGS-report-standard', 'PANKAJ', 'Microbial_genomics_Demo', 'ANISA', 'cache', 'Dr.Vivek', 'meeting_31-10-2023', 'Dr.Rakesh', 'Kalai_selvi', 'server', 'MISC', 'gatk-sv', 'BioPython_Module', 'Anshu', 'random', 'cnvkit', 'nextflow_scripts', 'Kraken_Reports', 'WGS', 'qiime _master_script.sh', 'TIDDIT', 'WGS-report-tools.docx', 'HiC', 'sratoolkit.3.0.6-ubuntu64', 'WGS_workshop', 'Untitled.ipynb', 'Sample_Metagenome_data', 'scripts', 'Clinical_exome_sequencing', 'SPAdes-3.15.5-Linux', 'blast-QC', 'Dr.Vinay_Tick_Borrelia', 'Dr.Sebastian', 'ML', 'methylC', 'breakdancer', '.ipynb_checkpoints', 'Sanger_Sequencing_Projects', 'Pendrive', 'Dr Shirish', 'Anju', 'Clinical_Genomics_Demo', 'brumir']



```python
#Creating a new Directory
#os.mkdir('/path/to/new/directory')
os.mkdir('/home/mediomix/Desktop/New_folder')
```


```python
#Removing a Directory
#os.rmdir('/path/to/directory')
os.rmdir('/home/mediomix/Desktop/New_folder/')

```

## re Module ( Regular Expression)

The re module in Python provides regular expression matching operations. Regular expressions (regex or regexp) are powerful tools for pattern matching and searching in strings. The re module allows you to work with regular expressions in Python. Here are some common functions provided by the re module:
1. re.search() \
The re.search() function searches for a specified pattern within a string. It returns a match object if the pattern is found, otherwise, it returns None.
2. re.match() \
The re.match() function checks if the pattern occurs at the beginning of the string. It returns a match object if the pattern is found at the beginning, otherwise, it returns None.
3. re.findall() \
The re.findall() function returns a list of all occurrences of the pattern in the string.
4. re.sub() \
The re.sub() function replaces occurrences of the pattern with a specified string.
5. Other Functions \
re.split(): Splits the string at each occurrence of the pattern. \
re.finditer(): Returns an iterator yielding match objects for all occurrences of the pattern.


```python
# re.search()
import re

pattern = r'apple'
text = 'I have an apple.'

match = re.search(pattern, text)

if match:
    print('Pattern found:', match.group())
else:
    print('Pattern not found.')

```

    Pattern found: apple



```python
# re.match()
import re

pattern = r'apple'
text = 'apple is a fruit.'

match = re.match(pattern, text)

if match:
    print('Pattern found at the beginning:', match.group())
else:
    print('Pattern not found at the beginning.')

```

    Pattern found at the beginning: apple



```python
# re.findall()
import re

pattern = r'\d+'  # Match one or more digits
text = 'There are 10 apples and 20 oranges.'

matches = re.findall(pattern, text)
print('Matches:', matches)

```

    Matches: ['10', '20']



```python
# re.sub()
import re

pattern = r'\d+'  # Match one or more digits
text = 'There are 10 apples and 20 oranges.'

modified_text = re.sub(pattern, 'X', text)
print('Modified Text:', modified_text)

```

    Modified Text: There are X apples and X oranges.



```python
#re.split()
import re

pattern = r'\s+'  # Match one or more whitespace characters
text = 'Split this text into words.'

words = re.split(pattern, text)
print('Words:', words)

```

    Words: ['Split', 'this', 'text', 'into', 'words.']


### Numpy 

NumPy, which stands for Numerical Python, is a powerful library in Python for numerical and mathematical operations. It provides support for large, multi-dimensional arrays and matrices, along with a collection of high-level mathematical functions to operate on these arrays. NumPy is a fundamental package for scientific computing in Python.

Here are some key features and aspects of NumPy:
* Arrays: The core feature of NumPy is the numpy.ndarray (n-dimensional array) data structure. This array is a table of elements, usually of the same type, indexed by a tuple of positive integers. NumPy arrays are more efficient than Python lists for numerical operations.
* Vectorized Operations: NumPy allows you to perform operations on entire arrays without the need for explicit loops. This is known as vectorization and is a key feature that makes NumPy powerful and efficient.
* Broadcasting: NumPy provides a mechanism called broadcasting that allows operations between arrays of different shapes and sizes.
* Mathematical Functions: NumPy includes a wide range of mathematical functions that operate element-wise on arrays, such as np.sin(), np.cos(), np.exp(), and more.
* Linear Algebra Operations: NumPy provides functions for linear algebra operations, including matrix multiplication (np.dot()), eigenvalue decomposition, and more.
* Random Number Generation: NumPy includes a subpackage numpy.random for generating random numbers.



```python
#Arrays
import numpy as np

# Creating a NumPy array
arr = np.array([1, 2, 3, 4, 5])
print(arr)
```

    [1 2 3 4 5]



```python
# Vectorized addition
result = arr + 10
print(result)
```

    [11 12 13 14 15]



```python
# Broadcasting example
arr1 = np.array([1, 2, 3])
arr2 = np.array([[10], [20], [30]])
result = arr1 + arr2
print(arr1)
print(arr2)
print(result)
```

    [1 2 3]
    [[10]
     [20]
     [30]]
    [[11 12 13]
     [21 22 23]
     [31 32 33]]



```python
# Mathematical functions
arr = np.array([1, 2, 3])
result = np.square(arr)
print(result)
```

    [1 4 9]



```python
# Matrix multiplication
matrix1 = np.array([[1, 2], [3, 4]])
matrix2 = np.array([[5, 6], [7, 8]])
result_dot = np.dot(matrix1, matrix2)
result_cross = np.cross(matrix1, matrix2)

print(result_dot)
print(result_cross)
```

    [[19 22]
     [43 50]]
    [-4 -4]



```python
# Random number generation
random_array = np.random.rand(3, 3)
print(random_array)
```

    [[0.02017728 0.08879981 0.78867674]
     [0.21658799 0.07673532 0.86514664]
     [0.96772185 0.56826858 0.15989148]]


## Pandas 

Pandas is a powerful open-source data manipulation and analysis library for Python. It provides easy-to-use data structures, such as Series and DataFrame, and functions designed for efficient data analysis and manipulation. Pandas is widely used in data science, machine learning, and other domains where data manipulation and analysis are crucial.
* DataFrame:The DataFrame is a two-dimensional, tabular data structure with labeled axes (rows and columns).It is similar to a spreadsheet or SQL table and can handle heterogeneous data types.DataFrames can be created from various data sources, including CSV files, Excel spreadsheets, databases, and more.
* Series:A Series is a one-dimensional labeled array capable of holding any data type.It is similar to a column in a DataFrame or a single column of data in a spreadsheet.
* Data Input/Output: Pandas supports reading and writing data in various formats, including CSV, Excel, SQL databases, JSON, and more.
* Data Cleaning and Transformation:Pandas provides functions for handling missing data, filtering, sorting, and transforming data.
* Indexing and Selection:Pandas allows for easy indexing and selection of data, making it convenient to extract specific subsets of a DataFrame.
* Grouping and Aggregation:Pandas supports grouping data by one or more columns and applying aggregate functions.
* Merging and Joining:Pandas provides functionality for combining multiple DataFrames based on common columns.


```python
# Creating a DataFrame
import pandas as pd

data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [25, 30, 35],
        'City': ['New York', 'San Francisco', 'Los Angeles']}

df = pd.DataFrame(data)
print(df)

```

          Name  Age           City
    0    Alice   25       New York
    1      Bob   30  San Francisco
    2  Charlie   35    Los Angeles



```python
# Creating a Series
ages = pd.Series([25, 30, 35], name='Age')
print(ages)
```

    0    25
    1    30
    2    35
    Name: Age, dtype: int64



```python
# Reading from CSV
df= pd.read_csv('iris.csv')
print(df)

# Writing to Excel
#df.to_excel('output.xlsx', index=False)

```

         sepal.length  sepal.width  petal.length  petal.width    variety
    0             5.1          3.5           1.4          0.2     Setosa
    1             4.9          3.0           1.4          0.2     Setosa
    2             4.7          3.2           1.3          0.2     Setosa
    3             4.6          3.1           1.5          0.2     Setosa
    4             5.0          3.6           1.4          0.2     Setosa
    ..            ...          ...           ...          ...        ...
    145           6.7          3.0           5.2          2.3  Virginica
    146           6.3          2.5           5.0          1.9  Virginica
    147           6.5          3.0           5.2          2.0  Virginica
    148           6.2          3.4           5.4          2.3  Virginica
    149           5.9          3.0           5.1          1.8  Virginica
    
    [150 rows x 5 columns]



```python
# Handling missing data
df.dropna()  # Drop rows with missing values
df.fillna(0)  # Fill missing values with a specified value

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>sepal.length</th>
      <th>sepal.width</th>
      <th>petal.length</th>
      <th>petal.width</th>
      <th>variety</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>5.1</td>
      <td>3.5</td>
      <td>1.4</td>
      <td>0.2</td>
      <td>Setosa</td>
    </tr>
    <tr>
      <th>1</th>
      <td>4.9</td>
      <td>3.0</td>
      <td>1.4</td>
      <td>0.2</td>
      <td>Setosa</td>
    </tr>
    <tr>
      <th>2</th>
      <td>4.7</td>
      <td>3.2</td>
      <td>1.3</td>
      <td>0.2</td>
      <td>Setosa</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4.6</td>
      <td>3.1</td>
      <td>1.5</td>
      <td>0.2</td>
      <td>Setosa</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5.0</td>
      <td>3.6</td>
      <td>1.4</td>
      <td>0.2</td>
      <td>Setosa</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>145</th>
      <td>6.7</td>
      <td>3.0</td>
      <td>5.2</td>
      <td>2.3</td>
      <td>Virginica</td>
    </tr>
    <tr>
      <th>146</th>
      <td>6.3</td>
      <td>2.5</td>
      <td>5.0</td>
      <td>1.9</td>
      <td>Virginica</td>
    </tr>
    <tr>
      <th>147</th>
      <td>6.5</td>
      <td>3.0</td>
      <td>5.2</td>
      <td>2.0</td>
      <td>Virginica</td>
    </tr>
    <tr>
      <th>148</th>
      <td>6.2</td>
      <td>3.4</td>
      <td>5.4</td>
      <td>2.3</td>
      <td>Virginica</td>
    </tr>
    <tr>
      <th>149</th>
      <td>5.9</td>
      <td>3.0</td>
      <td>5.1</td>
      <td>1.8</td>
      <td>Virginica</td>
    </tr>
  </tbody>
</table>
<p>150 rows × 5 columns</p>
</div>




```python
data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [25, 30, 35],
        'City': ['New York', 'San Francisco', 'Los Angeles']}

df = pd.DataFrame(data)

# Selecting columns
df['Name']

# Selecting rows based on condition
df[df['Age'] > 30]

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Age</th>
      <th>City</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2</th>
      <td>Charlie</td>
      <td>35</td>
      <td>Los Angeles</td>
    </tr>
  </tbody>
</table>
</div>



## Matplotlib

Matplotlib is a comprehensive 2D and 3D plotting library for Python. It produces high-quality static, animated, and interactive visualizations in Python. Matplotlib is widely used for creating a variety of plots and charts, making it an essential tool for data visualization and scientific computing.


```python
#Data Visualization using Matplotlib.pyplot
# Lineplots

import matplotlib
import matplotlib.pyplot as plt
matplotlib.use('TkAgg')
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

plt.plot(x, y)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Simple Line Plot')
plt.show()
```


```python
#Scatterplots
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

plt.scatter(x, y)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Scatter Plot')
plt.show()

```


```python
# Bar plot
import matplotlib.pyplot as plt

categories = ['A', 'B', 'C', 'D']
values = [3, 7, 1, 5]

plt.bar(categories, values)
plt.xlabel('Categories')
plt.ylabel('Values')
plt.title('Bar Plot')
plt.show()

```


```python
# Histogram
import matplotlib.pyplot as plt
import numpy as np

data = np.random.randn(1000)  # Random data

plt.hist(data, bins=30)
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.title('Histogram')
plt.show()

```


```python
# Pie chart
import matplotlib.pyplot as plt

labels = ['A', 'B', 'C', 'D']
sizes = [25, 30, 15, 30]

plt.pie(sizes, labels=labels, autopct='%1.2f%%')
plt.title('Pie Chart')
plt.show()

```


```python
# 3D scatter plot
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import Axes3D

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]
z = [1, 1, 2, 2, 3]

ax.scatter(x, y, z)
ax.set_xlabel('X-axis')
ax.set_ylabel('Y-axis')
ax.set_zlabel('Z-axis')

plt.show()

```
