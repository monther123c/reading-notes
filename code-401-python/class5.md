# Intro to OOP
---
# Classes and Objects
Class : a blueprint for objects. A class is a user-defined type that describes what a certain type of object will look like. A class description consists of a declaration and a definition. Usually these pieces are split into separate files.

An object is a single instance of a class. You can create many objects from the same class type.

An object consists of:

Name -- the variable name we give it Member data -- the data that describes the object Member functions -- behavior aspects of the object (functions related to the object itself)

Example of a class : in this example we created a new class called "Myclass" which now can be used to create objects out of it .This class contains one variable "new_variable" and one function "new_function".

Coverage :
How to get it
There's a package called pytest-cov on PyPI that you can download and install. Once that's done, you can invoke pytest with the --cov option. If you don't say anything more than that, you'll get a coverage report for every part of the Python library that your program used, so I strongly suggest you provide an argument to --cov, specifying which program(s) you want to test. And, you should indicate the directory into which the report should be written. So in this case, you would say:

" pytest --cov=mymul . "