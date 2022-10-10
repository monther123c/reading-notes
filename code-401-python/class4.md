# FileIO & Exceptions
---
## Read & Write Files in Python
First of all lets discuss what files are :
a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.
modern file systems are composed of three main parts:

Header: metadata about the contents of the file (file name, size, type, and so on)
Data: contents of the file as written by the creator or editor
End of file (EOF): special character that indicates the end of the file
Each file has its own unique path which has 3 parts :

Folder Path
File Name (Name in the picture below)
Extension (The last part of the file name after the separator)

----
# Exceptions in Python
An exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions.

ways to apply and exception in python :-
Default exception that can be Raised automatically
Cutomized exceptions that the developer can set when a specific senario happened
It is important to distinguish between two types of errors, syntax error result when the interpreter faces a Python code that is written in a wrong way, while, on the other hand, exception errors get raised when a correct python code causes an error, a typical example on that is when you try to open a file by specifying the file path wrongly.

To raise an exception, use the keyword raise followed by the function Exception().

Try and Except
Try and Except are used to handle errors manually (Exception errors) , We can use them to run a specific code in the try and handle any error with the excpet