class-03.md

## **Table Of Contents**

_Read:03_ HTML Lists, CSS Boxes, JS Control Flow

## ***Ducket HTML***

  1. Chapter 3: “Lists” (pp.62-73)
  2. Chapter 13: “Boxes” (pp.300-329)
  
## ***Ducket JS***
  
  1. Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)
  2. Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)

## HTML & CSS By Jon Duckett

### **Chapter 3: Lists**

- HTML has both ordered `<ol></ol>` and unordered `<ul></ul>` lists.
- Ordered lists will number the list items, where unordered lists will bullet the items.
- HTML also has definition lists. `<dl></dl>`, comprised of two elements internally. `<dt></dt>` Definition terms, and the definition its self `<dd></dd>`.
- Lists can also be nested inside of another list.

### **Chapter 13: Boxes**

- CSS sees HTML elements as boxes. You can manipulate these boxes with CSS.
- Using CSS you can set the dimensions of these boxes. Limit their width, height, and control the behavior of overflow content
- Every box has three properties which can be adjusted. The Border, the Margin, and Padding.
- Within these bounds there are many more CSS methods that can be applied to customize these properties.

## JS & Jquery By Jon Duckett

### **Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)**

- Arrays in JS are a special variable that can store multiple items, in indexed locations
- These locations can be called individually through the indexes. Starting at `0` being the first item in the array.

### **Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)**

- If Else statements can operate on a number of conditions. Using a if  > else if > else type structure.
- Each next step operating on a different condition, as long as the previous steps condition was not met.
- Switch statements start with a variable called a switch value. than execute code off of that value.
- If the switch value given to the statement does not match one of the 'Cases' inside the switch, than a default is run. Similar to an else in a if else loop.
- If not instructed otherwise with `use strict;` JS will attempt to change the type of a variable if it expected to receive a different data type.
- certain data types and values will evaluate as truthy and falsy. This is different than a concrete true or false value. I.e. `var num = 0;` is considered falsy.
- A loop in JS will check if a condition is true, and then execute code. If at any point that condition returns false. the loop will stop.
- A `for` loop is handy for running a specific block of code a set number of times.
- A `while` loop is great if you do not know how many times the loop will need to run.
- A `do while` loop is similar to a while loop, with one important difference. It will always run at least once. Even if the condition returns as false.
- Counters are a common method of controlling for loops. `for (var i = 0; i < 10; i++) {some code to execute}`. This line declares the `i` variable with a value of `0`, than checks that i  is less than 10. If so it executes the code, and adds 1 to the value of `i`.
- `break` is a very valuable keyword when working with loops, as it will stop a loop from running once the interpreter gets to it.
- Loops are a very helpful tool for iterating through an array.
