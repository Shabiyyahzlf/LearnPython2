# LearnPython2
## FUNCTION
- In mathematics, a function is a process that relates an input to an output. 
- In Python, besides serving as this mathematical relation, functions are also a way to organize code - with the ultimate goal of making the code reusable.
- Functions should ideally have a specific purpose but be reusable. 
- While Python provides many built-in functions, we can always define our own.
### Defining a function
- Functions are defined using the keyword "def" followed by the function name and its parameters in parentheses ().
- Optionally, you can add a docstring - a documentation string that explains the function's context.
- The block of code within each function starts with a colon: and uses indentation.
- A function terminates when there's a return [expression] statement, which returns the [expression] to the caller.
- You can also create functions that don't return an output by using return None.

<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/2261bace-c4de-4069-b53f-640b2727267e" /></div>
By default, Python will position each parameter according to the registration sequence when defined, and they must be called in that sequence.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/0f4bdca1-9bfe-43b4-bbfe-4303d523ff73" /></div>

### RETURN
The return [expression] statement will cause the program execution to exit from the function at that point, while also returning a specific value.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/ac54de37-ac42-4e30-8174-50f9a4f80c52" /></div>

- The return value of a function can be stored in a variable.
- This is what distinguishes a function that returns a value from one that does not (often referred to as a procedure).
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/d9205418-f2c1-42c6-9d12-62242d35ce14" /></div>

### DOT FORMAT¶
In Python, "dot format" commonly refers to the use of the format() method for string formatting. This method allows you to insert values into a string by specifying placeholders and providing the values to substitute.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/19acdcaf-33b5-4049-b963-3824a3db0b5b" /></div>

### Pass by Reference vs Value
- All parameters (arguments) in Python are "passed by reference". This means that when we modify a variable, the data referenced by it will also change, both inside the function and outside the calling function.
- Except if we perform an assignment operation that will change the reference parameter.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/57596891-071f-4d58-ab50-9ce233307632" /></div>

However, we must be careful because assigning a variable with the same name as a parameter creates a new variable in the local scope and is not related to the global variable.

## NUMPY
### What is NumPy?
NumPy is a Python library used for working with arrays. It also has functions for working in the domain of linear algebra, Fourier transform, and matrices. NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely. NumPy stands for Numerical Python.

At the core of the NumPy package, is the array object. This encapsulates n-dimensional arrays of homogeneous data types, with many operations being performed in compiled code for performance. There are several important differences between NumPy arrays and the standard Python sequences:
- NumPy arrays have a fixed size at creation, unlike Python lists. Changing the size of an array will create a new array and delete the original.
- The elements in a NumPy array are all required to be of the same data type and thus will be the same size in memory.
### The next step is how to apply NumPy in Python
### 1.Import and Checking NumPy Version
The “print(np.__version__)" syntax is used to determine the installed version of NumPy in Python.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/2ea5ab5b-97f0-47cf-88f5-bf48d5f37ba7" /></div>

### 2.Creating a NumPy Array
Next, we create a NumPy array using the np.array() function. We can pass a list [1,2,3,4,5] or a tuple (1,2,3,4,5) as arguments. This generates a one-dimensional array with elements matching the elements of the given list or tuple.

Then, we print the created array with "print(arr)" and print the data type of the array with "print(type(arr))". The result indicates that the created array is a numpy.ndarray object, which is a special data type provided by NumPy to represent multidimensional arrays.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/10d0082e-c578-4785-839f-16fa42d838f5" /></div>

### 3.DIMENSION
- The dimension in NumPy refers to the number of indices required to refer to an element in the array
#### Dimension in Arrays
A dimension in arrays is one level of array depth(inested arrays)

- ##### 0D arrays
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/2198768b-ba34-476c-8fce-ca9266df41d9" /></div>

- ##### 1 Dimension
  1D arrays in NumPy are essentially like lists in Python. They are sequences of elements arranged in a single line.
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/71606c1c-e9ec-44a2-b83a-2bd17942b6e3" /></div>
- ##### 2 Dimensions
  2D arrays in NumPy are like matrices. They have rows and columns, arranged in a grid format.
   <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/0ed18da5-1bc4-4da4-a062-81189a88c87f" /></div>
- ##### 3 Dimensions
  Creating a 3-dimensional array with two 2-dimensional arrays, both containing two arrays, can be achieved using NumPy as follows:
   <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/bd91ddc5-1bb8-4d6d-ba61-ba1b0fd0f184" /></div>
### 4.Check how many dimensions the arrays have
The "a = np.array" syntax is used to store an array variable in the NumPy library. The "print(a.ndim)" syntax is used to provide feedback by displaying dimensional information to the user.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/f30b5d7d-0005-4919-aa57-865eeaae74f3" /></div> 

### 5.Transforming Dimensions: Converting One Dimension to Another
Transforming one dimension into another dimension in NumPy involves modifying the shape or structure of an array, converting it from one dimension to a different dimension.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/8ca45164-3870-4779-a96f-3886d6a90c8a" /></div>

### 6.Get the results of the desired elements of the following array
- Get the first element from the following array
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/a2aadb22-b89b-413a-ac10-3bc154d41c28" /></div>
  To retrieve the first element, you use [0] because the indexing of elements starts from 0, then 1, 2, 3, etc.
- Get the second element from the following array
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/5d64196b-a4e5-408a-99ab-cfd9293a5f18" /></div>

- Get the third and fourth element from the following array
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/0a05d243-e366-4c28-9a0c-93f603d94b34" /></div>

  The "(fruits[2] + fruits[3])" syntax is used to find two elements, namely the third element and the fourth element.

### 7.Accessing elements from a specified array.
- Access the element on the 1st row, 2nd column
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/d5de6a13-b4f8-4995-80c8-a99a66bf195a" /></div>
  The "fruits[0, 1]" syntax is used to retrieve the element at 1st row and 2nd column.
- Access the element on the 2nd row, 5th column
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/510dd9ea-b4fc-4ff6-8157-f149348a89b5" /></div>
- Access the third element of the second array of the first array
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/27f439f7-b0da-424e-8d60-13a9de4d3dce" /></div>

#### TASK
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/b8d18cd3-29ed-4c33-aa02-81f4ee5505e1" /></div>
- 1 in the first dimension: Selects the second element in the first dimension, which is [[['Durian', 'Guava'], ['Avocado', 'Snake fruit']], [['Lychee', 'Papaya'], ['Melon', 'Kiwi']]].
- 0 in the second dimension: Selects the first row in the second dimension, which is [['Durian', 'Guava'], ['Avocado', 'Snake fruit']].
- 1 in the third dimension: Select the second element in that row, which is ['Avocado', 'Snake fruit'].
- 0 in the fourth dimension: Selects the first element in that row, 'Avocado'.

## PANDAS
Pandas is a powerful and widely used open-source Python library primarily used for data manipulation and analysis. It provides high-performance data structures and tools for working with structured data, making it an essential tool for data scientists and analysts.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/0ce9f0c8-fe5d-48ff-b1c0-3403df379e44" /></div>

Pandas has two main objects: Series and DataFrame.
### Series
The Series object is a ONE-dimensional array that can store various types of data, such as integers, floats, strings, and others. It does not have column names as it consists of only one column. Each element in a Series has a label called an index.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/f6d0e1f0-9144-4d12-8671-4ddf31a4f4ef" /></div>
Convert it into a Series
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/af9888e8-cb9c-48ff-aade-f52475ea1c3c" /></div>
Convert the Series to an array
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/3ae655ef-9e2b-436f-8d34-10a2da9b409b" /></div>

#### Indices
The indices are represented as a range, where the start point is inclusive, and the stop point is exclusive in the range.
- Implicit indexing: Default numerical index assigned based on positional order.
- Explicit indexing: Custom labels or values are assigned to uniquely identify rows or columns.
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/462368b4-20d2-4128-af5f-153b611ed0e2" /></div>
When the implicit and explicit indices are the same, when we call the data, it will rely only on its explicit indices.
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/41970891-eaac-49d0-b04d-0a9ad4761c63" /></div>
The result of name_2[0] is an error due to the similarity between the explicit indices and the implicit indices.

We'll now try to perform data-slicing
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/c7b87be4-dc4b-4343-85a1-2a237e681e66" /></div>
But if we slice its implicit indices, only the start point will appear, because implicit indices are in the form of a range
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/b8577ec1-81d3-417e-ac16-3ba49681a31d" /></div>

#### loc and iloc
Example of data where some implicit and explicit indices are the same.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/d463e103-0eab-4196-b3d9-6058be23acb0" /></div>
When we access a single index, it will display its explicit index.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/dc7f3cd7-3950-4976-b1f8-f8277f5b3948" /></div>
When explicit and implicit indices are the same, inconsistencies occur as in the case above.

To address this inconsistency, we will use the principles of loc and iloc.

loc is used to call its explicit indices, while iloc is used to call its implicit indices.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/10d07158-20b5-4c8f-af0b-58dca51493bf" /></div>

#### Dictionary--Series
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/5ae44f2d-fcb9-42b0-b3c0-c150052a9db7" /></div>

## DATAFRAME
Pandas introduces the DataFrame data structure, which is a two-dimensional tabular data structure with labeled axes (rows and columns). This allows for easy manipulation and analysis of data.

A DataFrame is a collection of Series, with at least one Series.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/e3dc51d1-169e-4ec4-9f44-26ff0b1a5734" /></div>
- When calling data with the syntax area_pop, it will appear as shown below.
- Because "pop" is the same as the function name in the DataFrame
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/0f37ca13-f591-4ea4-b490-e2060f6fbcee" /></div>
Therefore, it is safer to call the data using the syntax area['population'].
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/dedaa8cb-e122-44ca-a379-fbdf902741a4" /></div>
We'll change the column name "data" to "employee_1" and "data_2" to "employee_2"
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/8d07e0a5-c3cd-4699-8d10-15cea2d64520" /></div>

### Load Data CSV in Pandas
Import CSV files using the read_csv() function from the Pandas library. Set the column index when reading your data into memory, and ensure that the uploaded CSV data matches the folder.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/d31e29e2-db10-429c-8e21-6ec400932238" /></div>
- 1. df.info(): Memberikan informasi tentang DataFrame, termasuk jumlah baris dan kolom, tipe data setiap kolom, dan jumlah  nilai non-null dalam setiap kolom.
- 2. df.notnull(): Mengembalikan DataFrame dengan nilai boolean yang menunjukkan di mana nilai-nilai tidak null.
- 3. df.isnull(): Mengembalikan DataFrame dengan nilai boolean yang menunjukkan di mana nilai-nilai null.
- 4. df.sum(): Menghitung jumlah nilai di setiap kolom.
- 5. df.tail(): Mengembalikan 5 baris terakhir DataFrame secara default.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/1c63bfc5-f2b9-4a23-a2ef-5f2d0b804ce0" /></div>
- 6. df.shape: Mengembalikan tupel yang berisi jumlah baris dan kolom DataFrame.
- 7. df.columns: Mengembalikan daftar nama kolom DataFrame.
- 8. df.index: Mengembalikan indeks DataFrame.
- 9. df.describe(): Memberikan ringkasan statistik seperti jumlah, rata-rata, standar deviasi, nilai minimum, kuartil, dan nilai maksimum untuk setiap kolom numerik.
- 10. df.mean(): Menghitung rata-rata nilai untuk setiap kolom.
- 11. df.median(): Menghitung nilai median untuk setiap kolom.
- 12. df.mode(): Menghitung nilai modus untuk setiap kolom.
- 13. df.unique(): Mengembalikan array unik dari nilai yang ada dalam kolom.
- 14. df.nunique(): Mengembalikan jumlah nilai unik dalam setiap kolom.
- 15. df.value_counts(): Menghitung jumlah kemunculan setiap nilai dalam suatu kolom.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/fcde7f84-5da6-4bb4-84c4-c338e7259ca3" /></div>
Calling a Python dataset with terms and conditions means retrieving or selecting certain data from a dataset based on certain terms or conditions. This can be done using boolean operators or logical statements, such as ==, !=, <, >, <=, >=, or and, or, not.
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/b5546762-2203-4052-9d9c-a478d1df9a5b" /></div>
Calls several columns accompanied by a filter terms and conditions
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/7029a9b0-f813-4fe8-8fd7-7485270534be" /></div>

## RANDOM LIBRARY
The random module in Python provides various functions to generate random numbers. Here are some commonly used functions in the random library:
- random.random(): This function returns a random float number between 0.0 to 1.0
  <div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/268bd070-7599-419f-abfb-7e75ae34c540" /></div>

## DateTime
DateTime is a module in Python that deals with real-time data and time. It provides classes and functions to manipulate and format dates and times. Here are some commonly used classes and functions in the DateTime module.
- date : This class represents a date (year, month, and day) without time.
- datetime : This class represents a date and time (year, month, day, hour, minute, second, and microsecond).
- time : This class represents time (hour, minute, second, and microsecond) without a date.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/9c9f6906-8e10-4f65-b165-ebe4ddc4749e" /></div>

## LOAD DATA TXT
DateTime is a module in Python that deals with real-time data and time. It provides classes and functions to manipulate and format dates and times. Here are some commonly used classes and functions in the DateTime module.
### OPEN
In Python, you can open and read a text file using the built-in open() function. The open() function in Python is used to open a file and return a file (.txt) object.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/173deac9-86e6-4624-bafb-fa6191772580" /></div>

### READ
The read() function in Python is used to read the contents of a file object that has been opened using the open() function
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/d5eeed39-fa61-4747-a49e-caa078fc5519" /></div>

### CLOSE
The close() function in Python is used to close a file that has been opened using the open() function. This is important because it frees up system resources and ensures that any changes made to the file are saved.
<div align="center"><img src="https://github.com/Shabiyyahzlf/LearnPython2/assets/89763971/305bd811-01b4-4f86-827a-dd6efe93a01c" /></div>

