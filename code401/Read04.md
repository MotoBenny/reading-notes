# Read04
[classes and objects](https://www.learnpython.org/en/Classes_and_Objects)

#### Objects
- an collection of variables and functions
- inherits the variables and funtions from classes

#### Classes
A basic python class
```python
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()
```


### Accessing Object variables
Given the above defined class and object, we would do the following to access the variable within the object.
`myobjectx.variable`


## [Thinking Recursively](https://realpython.com/python-thinking-recursively/)

> If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.

^^^ This mindset, is what i need to remember to apply to every single part of my programming

### Maintaining state
Each recursive call has its own execution content. 
to maintain state within a recursive function you can
1) thread the state through each function call, so the state is part of the execution context
2) keep the state within global scope

# [Testing with Pytest](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

When writing tests aim to write a 'test suite' with individual tests working and testing each part of your code. 

In order to group these tests (often because this block of tests needs the sam variables, or pertains to the same functionality in the code) we can use `pytest.fixture`