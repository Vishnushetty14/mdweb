# Python Package
## In this article, you'll learn to divide your code base into clean, efficient modules using Python packages. Also, you'll learn to import and use your own or third party packages in a Python program.

# What are packages?
## We don't usually store all of our files on our computer in the same location. We use a well-organized hierarchy of directories for easier access.

## Similar files are kept in the same directory, for example, we may keep all the songs in the "music" directory. Analogous to this, Python has packages for directories and modules for files.

## As our application program grows larger in size with a lot of modules, we place similar modules in one package and different modules in different packages. This makes a project (program) easy to manage and conceptually clear.

![Alt text](https://www.python-course.eu/images/packages.webp "a title")

## Similarly, as a directory can contain subdirectories and files, a Python package can have sub-packages and modules.

## A directory must contain a file named init.py in order for Python to consider it as a package. This file can be left empty but we generally place the initialization code for that package in this file.

## Here is an example. Suppose we are developing a game. One possible organization of packages and modules could be as shown in the figure below.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2018/02/Package-Module-Structure.png)

## Importing a Python Package We’ll import a package using the import statement:
![](https://www.udacity.com/blog/wp-content/uploads/2021/01/Screen-Shot-2021-01-04-at-2.25.10-PM.png.webp)

## Let’s assume that we haven’t yet installed any packages. Python comes with a big collection of pre-installed packages known as the Python Standard Library. It includes tools for a range of use cases, such as text processing and doing math. Let’s import the latter:
# Packages
## Numpy
### Numpy is a popular Python array processing package. It provides good support for different multidimensional array objects. Numpy is not only limited to providing arrays, but also provides a variety of tools for managing these arrays. It is fast, efficient and very good for managing arrays and arrays.
#


## OpenCV Python
### OpenCV, also known as ** Open Source Computer Vision **, is a package for image processing. It monitors general functions focused on the instant view of the computer. Although OpenCV does not have adequate documentation, according to many developers, it is one of the hardest libraries to learn. However, it provides many built-in functions through which you learn computer vision easily.
![](https://en.terminalroot.com.br/assets/img/python/opencv-python-library.jpg)

#
## Mathematical functions
### This module provides access to the mathematical functions defined by the C standard.These functions cannot be used with complex numbers; use the functions of the same name from the cmath module if you require support for complex numbers. The distinction between functions which support complex numbers and those which don’t is made since most users do not want to learn quite as much mathematics as required to understand complex numbers. Receiving an exception instead of a complex result allows earlier detection of the unexpected complex number used as a parameter, so that the programmer can determine how and why it was generated in the first place.

### __ex__:- _math.ceil(x)_
### _Return the ceiling of x, the smallest integer greater than or equal to x. If x is not a float, delegates to x.__ceil__(), which should return an Integral value._

## A More Complex Package
### We will demonstrate in the following example how we can create a more complex package. We will use the hypothetical sound-Modul which is used in the official tutorial.
`
sound
|-- effects
|   |-- echo.py
|   |-- __init__.py
|   |-- reverse.py
|   `-- surround.py
|-- filters
|   |-- equalizer.py
|   |-- __init__.py
|   |-- karaoke.py
|   `-- vocoder.py
|-- formats
|   |-- aiffread.py
|   |-- aiffwrite.py
|   |-- auread.py
|   |-- auwrite.py
|   |-- __init__.py
|   |-- wavread.py
|   `-- wavwrite.py
`-- __init__.py `
