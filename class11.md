# summery 
# JupyterLab
___
![image](https://miro.medium.com/max/740/1*pmrv_BOroLiBBMWcU3TMzw.png)
- JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner. For a demonstration of JupyterLab and its features, you can view this video:

- JupyterLab is a next-generation web-based user interface for Project Jupyter.

- You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing, for example:

- JupyterLab also offers a unified model for viewing and handling data formats. JupyterLab understands many file formats (images, CSV, JSON, Markdown, PDF, Vega, Vega-Lite, etc.) and can also display rich kernel output in these formats. See File and Output Formats for more information.

- JupyterLab extensions can customize or enhance any part of JupyterLab, including new themes, file editors, and custom components.

- JupyterLab is served from the same server and uses the same notebook document format as the classic Jupyter Notebook.




# NumPy 
![image1](https://miro.medium.com/max/765/1*cyXCE-JcBelTyrK-58w6_Q.png)
NumPy is a python library used for working with arrays. It also has functions for working in domain of linear algebra, fourier transform, and matrices.

Numpy is a general-purpose array-processing package. It provides a high-performance multidimensional array object, and tools for working with these arrays. It is the fundamental package for scientific computing with Python.


Array in Numpy is a table of elements (usually numbers), all of the same type, indexed by a tuple of positive integers. In Numpy, number of dimensions of the array is called rank of the array.A tuple of integers giving the size of the array along each dimension is known as shape of the array. An array class in Numpy is called as ndarray. Elements in Numpy arrays are accessed by using square brackets and can be initialized by using nested Python Lists.


#### Creating a Numpy Array

Arrays in Numpy can be created by multiple ways, with various number of Ranks, defining the size of the Array. Arrays can also be created with the use of various data types such as lists, tuples, etc. The type of the resultant array is deduced from the type of the elements in the sequences.

    
    import numpy as np
    
    
    arr = np.array([1, 2, 3])
    print(arr)
    
    
    # Creating an array from tuple
    arr = np.array((1, 3, 2))
    print("\nArray created using "
        "passed tuple:\n", arr)


Output:

    
    [1 2 3]
    
    Array created using passed tuple:
    [1 3 2]


* With NumPy, we can work with multidimensional arrays.we’ll focus on 2-dimensional arrays. A 2-dimensional array is also known as a matrix or ( list of lists). A matrix 
has rows and columns.By specifying a row number and a column number, we’re able to extract an element from a matrix.
* the core of NumPy is written in a programming language called C, which stores data differently than the Python data types. NumPy data types map between Python and C, allowing
us to use NumPy arrays without any conversion hitches.
* NumPy has several different data types, the important ones are :
  * `float` — numeric floating point data.

  * `int` — integer data.
  * `string` — character data.
  * `object` — Python objects

* NumPy makes it simple to perform mathematical operations on arrays. This is one of the primary advantages of NumPy, and makes it
quite easy to do computations.

* NumPy makes it possible to test to see if rows match certain values using mathematical comparison operations like `<, >, >=, <=, and ==`
* With NumPy, it’s very common to combine multiple arrays into a single unified array

