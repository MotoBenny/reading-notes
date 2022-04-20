# Read03

[Read and Write files with python](https://realpython.com/read-write-files-python/)

[Video](https://realpython.com/lessons/opening-and-closing-files/)

- files in python are opened with `file = open("text_file.txt")`
	- takes a file name or path as argument
- files need to be closed when finished being ysed file.close()


## Example useage

```python
file = open("file.txt")
try:
	#Logical processing of file/editing or adding to file
finally:
	file.close()
```

## alternatively 
- use the with open("file.txt")  as file:

``` python
with open('file.txt')
	# process the file as needed
	
#file is automatically closed when using with
```

# Opening files

##### Write mode

open("filename.txt", "w")

##### Read mode

open("filename.txt", "r")  
open("filename.txt")

##### Binary Write mode

open("filename.txt", "wb")

-   Binary write is used for non text files. like Images or Sound files.
    
-   you can pass in a + along with any of the mode arguments, to extend their function. I.e. open a document with read and write capabilities
    
-   open("filename.txt", "r+")
    

---

# Closing files

text_file.close()

---

# Reading files

file = open("filename.txt", "r")  
content = file.read()  
print(content)  
file.close()

-   .read() can be tossed a number argument which is the number of bytes it should read from that file.

---

# Writing files

file = open("filename.txt", "r")  
file.write("This has been written to file")  
file.close()

When a file is opened in write mode, its existing content is deleted.

-   the write method returns the number of bytes written to the file if it succeeds
___

## [Python Exceptions](https://realpython.com/python-exceptions/)

An exception error occures when syntactically correct python code results in an error.

## Raising an #Exception[](https://realpython.com/python-exceptions/#raising-an-exception "Permanent link")

We can use `raise` to throw an #exception if a condition occurs. The statement can be complemented with a custom exception.
```
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

### We can use AsserttionError 
To assert that a condition is met, If this condition evaluates to false, we can throw an error.

---
>## The `try` and `except` Block: Handling Exceptions[](https://realpython.com/python-exceptions/#the-try-and-except-block-handling-exceptions "Permanent link")
>
>The `try` and `except` block in Python is used to catch and handle exceptions. Python executes code following the `try` statement as a “normal” part of the program. The code that follows the `except` statement is the program’s response to any exceptions in the preceding `try` clause.
>
>[![Diagram showing try and except statements](https://files.realpython.com/media/try_except.c94eabed2c59.png)](https://files.realpython.com/media/try_except.c94eabed2c59.png)
>
>As you saw earlier, when syntactically correct code runs into an error, Python will throw an exception error. This exception error will crash the program if it is unhandled. The `except` clause determines how your program responds to exceptions.

Taken from [RealPython.com](https://realpython.com/python-exceptions/)
___

## Else

An else caluse can be used with a try: except: block, to run code if no exceptions are thrown.

## Finally 

Finally is run after all other code, A finally statement will always run, regardless of what happens within the try/except/else blocks.