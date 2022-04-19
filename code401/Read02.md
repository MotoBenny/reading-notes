# Read:02

### [In Tests We Trust - TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
---
#### #Unit-tests
Code written to test the input/output and general behavior of your code.
	- for instance does this function return the expected data type?
	- When this function is called, is it receiving what I expext as an argument?
	
These sorts of tests can find and fix bugs before they happen, and in my experience help to cement exactly what each portion of your code should be doing/returning.
To an extent well written unit tests provide a roadmap for what your code should be doing, and what you should program next.

#### #TDD #test-driven-development
A style of programming where you begin by designing a suite of tests based on the intended funciton, than build your program to ensure those tests pass. 

- TDD will see you breaking your code down into its smallest reasonable component parts. 

---
#### Tests naming structure
``` File structure of tests and naming
mymodule/
	— module.py 
	— another_folder/
	— — another_module.py
tests/ 
	— test_module.py 
	— another_folder/
	— — test_another_module.py
```
---


#### Test structure
A common structure is AAA:
**Arrange, Act, and Assert**

* Arrange: organize the data you need to execute the code you are testing, Get the required input.
* Act: execute the code
* #Assert: Check the result is what you were expecting

---

#### the steps/Cycle
1) Write a unit test and make it fail (it will fail because the functionality its testing doesnt exsist yet)
2) Write the functionality in the code, and ensure the test passes.
3) Refactor the code for readability and efficency

___

### main points of TDD
1) Design the software before you write the software.
2) Your code will be reliable
---

## If \__name__ == "\__main\__":
* Tells the python interpreter if this application is the main body of our application
	- Which determines if it runs through all the code, or simple initializes it and defines the functions/variables for later use.
* Allows us to import our code as a module in another application or script, and access the functions therein. 

## #Recursion
"**What is Recursion?**   
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function." - Geeksforgeeks.org/recursion

Recursive functions are much more adaptable and efficent, but can cause stack overflow if the base case is never reached. 

[Recursion](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

