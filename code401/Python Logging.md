#logging
#python

# Logging to debug in python

- Logging is a native python module, No install or reqs, Simply import logging like so

```python
import logging
```

### Levels of Logging

- loging.debug()
- logging.info()
- logging.warning()
- logging.error()
- logging.critical()

```python
import logging

basicConfig(level=logging.debug)
# this means that anything from the debug level or higher (which is all other levels) will be logged
```

By default terminal output will only include warning or higher level logs.

Including these with the properties and values you are interacting with at that point in your program will allow you to easily see how they change during the flow of your application. But this isnt much different to simply printing the variables.

So lets log them to a specific log file!

### Logging to a file
Logging to a file will allow us to examine and reference how the things we pass into our log change through the flow of an application. 
- example:
	- If we log all the variables each of our functions interacts with as the function is called, along with a quick message to label the log to attach it to that function, we can easily see how our data morphs and changes as each function is called, this will make it easy to see how the data changes as the application flows, allowing us to see where things are starting to go sideways! 
		- Why did my variable 'x' suddenly get 200 bigger within my dont_add_200_to_x() function, that shouldnt be happening!

```python
import logging

basicConfig(level=logging.INFO, filename="log.log", filemode='w')
# lets break this down
# level: sets what level of log (and higher) we will write to log
# filename: The name of your log file, consider projectname.log
# filemode: standard python file modes here, "w" means write a file, and if one already exsists overwrite it. 

```
