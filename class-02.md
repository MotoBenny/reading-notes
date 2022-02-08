Class-02.md

## **Table Of Contents**

_Read:02_ HTML Text, CSS Introduction, and Basic JavaScript Instruction

## ***Ducket HTML***

  1. HTML Chapter 2: "Text" 
  2. HTML Chapter 10: "Introducing CSS"

## ***Ducket JS***

  1. JS Chapter 2: "Basic Javascript instructions"
  2. JS Chapter 4: "Decisions and loops"

## HTML & CSS By Jon Ducket

### **Chapter 2: "Text"**

  - Structural markup: The HTML elements used to describe the headings and paragraphs
  - Semantic markup: The HTML elements which provides extra information/formatting, such as italics, or a quote and who said it.

### Some HTML Elements

  1. `<h1> through <h6>` Header elements, with `<h1></h1>` being the largest, and `<h6></h6>` being the smallest.
  2. `<p></p>` Paragraph elements.
  3. `<b></b>` Bold elements.
  4. `<i></i>` Italic elements.
  5. `<sup></sup>` Superscript, used for things like dates or number exponents i.e. the 4<sup>th</sup> of the month.
  6. `<sub></sub>` Subscript, used for subscript such as H<sub>2</sub>O.

### Some Semantic HTML Elements

  1. `<strong></strong>` Strong, indicates importance of the words within. Browsers will also <b>Bold</b> the contents.
  2. `<em></em>` Emphasis, Subtle changes to the meaning of a sentence. Browsers display this as <i>Italics</i>.
  3. `<blockquote></blockquote>` Is used for long quotes, such as an entire paragraph. Browsers most often indent the contents.
  4. `<q></q>` Quote, is used for quotes contained inside a `<p>` paragraph. Most browsers will put " marks around these.
    - Both quote and blockquote can use the attribute `cite=""` to cite the quote with a URL.
  
 - There are many more specific elements that can modify or provide extra context to your HTML.

### **Chapter 10: "introducing CSS"**

  - CSS or cascading Style Sheets, allows you to select a specific element and assign rules that denote how it should be displayed.
  - Using a structure of a selector (this is the actual HTML element such as `<p>`) followed by a declaration 
  (the rules that denote how the browser should style that element such as `{ color: Blue; }`) 

  - CSS can be applied to an HTML document either by linking to the CSS file.
   Or locally within the HTML itself within `<style></style>` Tags.

## Javascript and Jquery By Jon Ducket

### **Chapter 2: "Basic Javascript instructions"**

  - `var let or const` to declare a variable 
  - once declared you can assign a value to the variable with the `=` sign.
  - an Array stores a list of variables `colors = ['white','blue','orange']; `
  - standard arithmetic operators apply, with a couple stand outs. ` ++ ` is to increment a value by +1, and `--` to decrement a value -1.

### **Chapter 4: "Decisions and Loops"**

  - Loops allow you to iterate over a section of code based on a certain condition. i.e. as long as variable A is less than 5 execute this code block.
  - Logical operators and Comparison operators will return a Boolean value of `true` or `false`.
  - If and If Else statements allow you to further your comparison and loop structure.
  - `if (condition = true) { perform this code; } else {perform this code;}`