Class-02.md

## **Table Of Contents**

_Read:02_ HTML Text, CSS Introduction, and Basic JavaScript Instruction

## ***Ducket HTML***

  1. HTML Chapter 2: "Text" 
  2. HTML Chapter 10: "Introducing CSS"

## ***Ducket JS***

  1. JS Chapter 2: "Basic Javascript instructions"
  2. JS Chapter 4: "Decisions and loops"

## HTML & CSS By Jon Duckett

### **Chapter 2: "Text"

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
  2. `<em></em>` Emphasis, Subtle changes to the meaning of a scentence. Browsers display this as <i>Italics</i>.
  3. `<blockquote></blockquote>` Is used for long quotes, such as an entire paragraph. Browsers most often indent the contents.
  4. `<q></q>` Quote, is used for quotes contained inside a `<p>` paragraph. Most browsers will put " marks around these.
    - Both quote and blockquote can use the attribute `cite=""` to cite the quote with a URL.
  
 - There are many more specific elements that can modify or provide extra context to your HTML.

 ### **Chapter 10: "introducing CSS"

  - CSS or cascading Style Sheets, allows you to select a specific element and assign rules that denote how it should be displayed.
  - Using a structure of a selector (this is the actual HTML element such as `<p>`) followed by a declaration 
  (the rules that denote how the browser should style that element such as `{ color: Blue; }`) 

  - CSS can be applied to an HTML document either by linking to the CSS file.
   Or locally within the HTML itself within `<style></style>` Tags.