# Introduction to Numpy

### What is Numpy ?
* NumPy is the fundamental package for scientific computing in Python. It is a Python library that provides a multidimensional array object, 
various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, 
sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more.

* Our Python NumPy Tutorial provides the basic and advanced concepts of the NumPy. Our NumPy tutorial is designed for beginners and professionals.
NumPy stands for numeric python which is a python package for the computation and processing of the multidimensional and single dimensional array elements.

* Travis Oliphant created NumPy package in 2005 by injecting the features of the ancestor module Numeric into another module Numarray.
It is an extension module of Python which is mostly written in C. It provides various functions which are capable of performing the numeric computations with a high speed.
NumPy provides various powerful data structures, implementing multi-dimensional arrays and matrices. These data structures are used for the optimal computations regarding
arrays and matrices.

### The need of NumPy
With the revolution of data science, data analysis libraries like NumPy, SciPy, Pandas, etc. have seen a lot of growth. With a much easier syntax than other programming languages, python is the first choice language for the data scientist.
NumPy provides a convenient and efficient way to handle the vast amount of data. NumPy is also very convenient with Matrix multiplication and data reshaping. NumPy is fast which makes it reasonable to work with a large set of data.

There are the following advantages of using NumPy for data analysis.

* NumPy performs array-oriented computing.
* It efficiently implements the multidimensional arrays.
* It performs scientific computations.
* It is capable of performing Fourier Transform and reshaping the data stored in multidimensional arrays.
* NumPy provides the in-built functions for linear algebra and random number generation.
* Nowadays, NumPy in combination with SciPy and Mat-plotlib is used as the replacement to MATLAB as Python is more complete and easier programming language than MATLAB.

### NumPy Environment Setup
NumPy doesn't come bundled with Python. We have to install it using the python pip installer. Execute the following command.
```
pip install numpy 

```

### Creating Arrays in Numpy 

```
import numpy as np
arr = np.array([1,2,3,4,5,6,7,8,9,10])

```

### Array Dimensions

1. 0-D Arrays

```
arr = np.array(42)
```

2. 1-D Arrays

 ```
 arr = np.array([1,2,3,4,5,6,7,8,9,10])
 ```
 
 3. 2-D Arrays
 
 ```
 arr = np.array([[1,2,3,4],[5,6,7,8]])
 ```
 
 4. 3-D Arrays
 ```
 arr = np.array([[[1,2,3],[4,5,6]],[[7,8,9],[10,11,12]]])
 ```
 
 ### Numpy Array Slicing :
 
 * Slicing in python means taking elements from one given index to another given index.
 * We pass slice instead of index like `[start:end]`
 * We can also define the step like `[start:end:step]`
 * If we don't pass start, start is considered 0
 * If we don't pass end , it is considered as last element of the dimension
 * If we don't pass step, it is considered to be 1
 
 ```
arr = np.array([1, 2, 3, 4, 5, 6, 7])
arr[1:5]
arr[4,:]
arr[:,4]
arr[-3:-1]
arr[::2]
arr[1,2:5]
arr[0:2,1:3]
 ``` 
 ### Data Types in Numpy

* i - Integer
* b - Boolean
* u - Unsigned Integer
* f - Float
* c - Complex Float
* m - Timedelta
* M - Datetime
* O - Object
* S - String 
* U - Unicode String
* V - Fixed chunk of memory for other type

### Shape of an array

* The shape of an array is the number of elements in each dimension.
* It can be determined using `arr.shape`
* Integers at every index tells about the number of elements the corresponding dimension has.


### Joining Numpy Arrays

* Joining means putting contents of two or more arrays in a single array.
* In SQL we join tables based on a key, whereas in NumPy we join arrays by axes.
* We pass a sequence of arrays that we want to join to the `concatenate()` function, along with the axis. If axis is not explicitly passed, it is taken as 0.

**Example 1**
```
arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.concatenate((arr1, arr2))

```

**Example 2**
```
arr1 = np.array([[1, 2], [3, 4]])

arr2 = np.array([[5, 6], [7, 8]])

arr = np.concatenate((arr1, arr2), axis=1)
 
 ```

**Example 3**
```
numpy.concatenate() with axis=0
import numpy as np  
x=np.array([[1,2],[3,4]])  
y=np.array([[12,30]])
z=np.concatenate((x,y), axis=0)  
z
```
 **Example 4**
 ```
numpy.concatenate() with axis=1
import numpy as np  
x=np.array([[1,2],[3,4]])  
y=np.array([[12,30]])  
z=np.concatenate((x,y.T), axis=1)  
z  
```


### numpy.append() in Python
The numpy.append() function is available in NumPy package. As the name suggests, append means adding something.
The numpy.append() function is used to add or append new values to an existing numpy array. This function adds the new values at the end of the array.
The numpy append() function is used to merge two arrays. It returns a new array, and the original array remains unchanged.

# Syntax
* numpy.append(arr, values, axis=None)  

 **Example 1**
```
np.append()
import numpy as np  
a=np.array([[10, 20, 30], [40, 50, 60], [70, 80, 90]])  
b=np.array([[11, 21, 31], [42, 52, 62], [73, 83, 93]])  
c=np.append(a,b)  
c
```

**Example 2**
```
#np.append({a1,a2,...}, axis=0)
import numpy as np  
a=np.array([[10, 20, 30], [40, 50, 60], [70, 80, 90]])  
b=np.array([[11, 21, 31], [42, 52, 62], [73, 83, 93]])  
c=np.append(a,b,axis=0)  
c 
```

**Example 3**
```
np.append({a1,a2,...}, axis=1)
import numpy as np  
a=np.array([[10, 20, 30], [40, 50, 60], [70, 80, 90]])  
b=np.array([[11, 21, 31], [42, 52, 62], [73, 83, 93]])  
c=np.append(a,b,axis=1)  
c
```

### numpy.sum() in Python
The numpy.sum() function is available in the NumPy package of Python. This function is used to compute the sum of all elements, the sum of each row, and the sum of each column of a given array.
Essentially, this sum ups the elements of an array, takes the elements within a ndarray, and adds them together. It is also possible to add rows and column elements of an array.
The output will be in the form of an array object

![image](https://user-images.githubusercontent.com/84801896/123977559-b6edc380-d9dc-11eb-8b72-cf25468012b4.png)
### Syntax
There is the following syntax of numpy.sum() function:
numpy.sum(arr, axis=None, dtype=None, out=None, keepdims=<no value>, initial=<no value>) 
  
  
**Example 1**
 ```
numpy.array()
import numpy as np  
a=np.array([0.4,0.5])  
b=np.sum(a)  
b  
```
**Example 2**
 ```
import numpy as np  
a=np.array([0.4,0.5,0.9,6.1])  
x=np.sum(a, dtype=np.int32)  
x 
  
 ```
  
### numpy.zeros() in Python
The numpy.zeros() function is one of the most significant functions which is used in machine learning programs widely. This function is used to generate an array containing zeros.
The numpy.zeros() function provide a new array of given shape and type, which is filled with zeros.
  ![image](https://user-images.githubusercontent.com/84801896/123979062-041e6500-d9de-11eb-860a-86ba6ebb55bc.png)
  ### Syntax
* numpy.zeros(shape, dtype=float, order='C'  
  
  **Example 1**
   ```
  numpy.zeros() without dtype and order
  import numpy as np  
  a=np.zeros(6)  
  a  
   ```
  **Example 2**
  
   ```
  numpy.zeros() with shape
  import numpy as np  
  a=np.zeros((6,2))  
  a  
  
   ```
 
  **Example 3**
  ```
  numpy.zeros() with the shape
  Import numpy as np  
  s1=(3,2)  
  a=np.zeros(s1)  
  a  
   ```
  




