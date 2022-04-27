# Big0 

a list is a stack of books,

# O(1) - always takes the same ammount of effort
If you want to put a new book on top of the stack (adding to the end of a list)
	- put the book on top of the book
	- this is always the same, takes the same ammount of effort, just add the book to the end of the stack

# O(n) - changes based on how many books there are in the stack
- If you want to put a book under the stack
	- You have to lift up the previous book,
	- and this getts harder since you are lifting more books each time


## BigO

#Time_Complexity - How many steps or times the algorithm (function) needs to run to complete a given task

#number_of_instructions - the number of inputs has an effect on how long the algorithm runs ( in the case of bigO this is refered to as 'n' )

---
Big-O notation is always for a given worst case - the maximum possible steps to complete a function

![[https://miro.medium.com/max/1400/1*PNttU1Wgihyk2ppJqWlvFg.png]]

#Logarithmic - an algoritm that reduces the size of the input data with each step.
	- i.e. binary search - O(log n)
	
#Linear_Time - The algorithms running time increases linearly as the size of the input data increases. - O(n)

#Quasilinear_Time - If your function references another funciton with linear time complexity ( binary search ) you must account for that when computing its BigO
ex: Your function requires a binary search to be performed on 15 data sets, to get 15 unique values, to perform an opperation on. - O(n Log n)

```python

"our string"
#0123456789 index

[:4] < Grab all index values from 4 to the begining of the string
[4:] < grab all index values from 4 to the end of the string

[1, 5, 6, 2, 6]

```