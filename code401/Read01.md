# Read:01

### Pain Vs Suffering

- This is going to be hard, very hard. 401 will take more concentration and effort than likely 301 and 201 combined. 
	- Ill need to seriously #timebox, I wont be able to afford time spent stuck.
	How will I ensure I continue to press on and solve problems?
	1) I will recognize when I am stuck and ask for help early and often.
	2) I will break down problems into their smallest component parts, solving each part as I best understand how.
	3) I will note when and how I become stuck or things I struggle with, and review them later to note how I resolved the problem. Commiting my solution to memory, hopefully to avoid that problem again. 

- This learning will be difficult and frustraighting. It will often suck, and drain me of energy, but recognizing that the learning and end product of this effort and frustraition will be difficult will allow me to push on, and succeed. 

___

### [[Big O]]
[Big O](https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation)

CS notation relating to the performance or complexity of an algorithm

1)  O(1)
	- an [[algorithm]] that will aleays excute the same time (or space) regardless of the size of the input data set.

2) O(N)
	- #Algorithm whose performance will grow linearly in proportion to the size of the data input. 
	- For instance this describes the upper limit for say how long (how many itterations) an algoritm will run for.

3) O(N<sup>2</sup>)
	- an algorithm whose performance. is directly related to the square of the size of the input data. Nested itterations over a data set will fit this descriptor. Deeper nestings increase the sqare number. O(<sup>3</sup>) and so on.

4) O(2^N)
	- Algorithm whose growth doubles with each addition to the input. The growth curve is exponential, A prime example is a recursive function calculating the Fibbonacci numbers. Example in JS :
```JS
int Fibonacci(int number)
{
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
}
```


### #Logarithms

> [[Binary search]]

>> "Binary search is a technique used to search sorted data sets. It works by selecting the middle element of the data set, essentially the median, and compares it against a target value. If the values match, it will return success. If the target value is higher than the value of the probe element, it will take the upper half of the data set and perform the same operation against it. Likewise, if the target value is lower than the value of the probe element, it will perform the operation against the lower half. It will continue to halve the data set with each iteration until the value has been found or until it can no longer split the data set.  
This type of algorithm is described as O(log N). The iterative halving of data sets described in the binary search example produces a growth curve that peaks at the beginning and slowly flattens out as the size of the data sets increase e.g. an input data set containing 10 items takes one second to complete, a data set containing 100 items takes two seconds, and a data set containing 1,000 items will take three seconds. Doubling the size of the input data set has little effect on its growth as after a single iteration of the algorithm the data set will be halved and therefore on a par with an input data set half the size. This makes algorithms like binary search extremely efficient when dealing with large data sets."

___

### Python Names and Values
[Facts and Myths about Python Names and Values.](https://www.youtube.com/watch?v=_AEJHKGk9ns)

#### Video Notes. 

* Names refer to values. 
* many names can refer to one value. If x = 23 and y = x than y = 23
* changing the value of x will not then change the value of y, y will still = 23
* Assignment never copies data 
``` python
nums = [1, 2, 3]
other = nums
# other and nums are both a list, containing 1, 2, 3 at this point.

nums.append(4)
print(other)  #[1, 2, 3, 4]
# because other = nums, if you append to nums, other is updated as it references that list.
```
[[mutable aliasing]]

#### [[immutable]] values
 Values that cannot be changed in place.
 Ints, floats, strings, tuples
 no methods that will let you change immutable values.
 
 ``` python
x = "Hello"
y = x
x = x + " there"
print(x) # "Hello there"
print(y) # "Hello"
```

- change is confusing, instead rebind.
``` x = x + 1 ``` This doesnt change X it rebinds it
changing a list
``` nums.append(7)``` This changes the list adding a value to it

Mutable and immutable calues are assigned the same
* Assignment is the same for all values.
* Aliasing can make it seem different. 

Function arguments are assignments

##### Best way to avoid mutable aliasing dont mutate values, Make new values. 

- names have no type
- values have no scope

[[Handy Tools]]