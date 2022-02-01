Class-01.md

## **Table Of Contents**

_Read:01_ Introductory HTML and Javascript

## ***Ducket HTML***

  1. HTML Introduction
  2. HTML Chapter 1: "Structure"
  3. HTML Chapter 8: "Extra Markup"
  4. HTML Chapter 17: "HTML5 Layout"
  5. HTML Chapter 18: "Process & Design"
  
## ***Ducket JS***
  
  1. JS Introduciton
  2. JS Chapter 1: "The ABC of Programming"

## HTML & CSS By Jon Duckett

### **Introduction**

- HTML is the meat (or other protien if you prefer) of your webpage. Its the content and basic structure that establishes what will be displayed by the browswer. It Creates a known structure that we can then access and continue to modify/customize with other tools, such as CSS or JS.

### **Chapter 1: Structure**

- HTML is made up of various elements which will have a opening and closing tag, the content of the page goes between these tags, and the tags will denote the basic styling for the content.
- Example  `<h1> Heading 1 </h1>` This is a heading tag, it happens to be heading 1, which is the largest of the available heading tags. There are a total of 6 heading tags from `<h1> to <h6>`.
- These tags can further be customized by adding atrribute names and values, These tags tell the browser certain important information about the content inside the tags.
- HTML uses many different tags to manage content. Most of these tags will have both and opening and closing tag, but not everyone.

### **Chapter 8: "Extra Markup"**

- The `<!Doctype html>` Tag tells the web browser to expect HTML following that tag.
- `<!-- Note goes here -->` This is the syntax for a note in HTML. Notes could handily be placed between important transitions on your webpage, for example where your introduction ends and the main content begins. These comments will only be visiable in the source for the page. And therefore are to help with readablility and understanding when modifying or examining the HTML later.
- Every HTML tag can have an id attribute. This is a unique identifier that can only be used on that single tag, but will allow you to address that tag in future code, perhaps to assign certain styling with CSS, or to link to that content from a different location on the page. Again, No two tags or elements may share the same ID attribute.
- Every HTML tag can also have a class attribute. Think of this like a ID attribute only a class can be assigned to multiple tags. Which can be addressed later as a group, to apply certain styling and more.
- Block elements in HTML will modify the basic formating of the HTML. I.E. a unordered list `<ul></ul>` will create a block on the page that contains its content.
- In line elements will not reformat the page content. Examples of these include `<em></em>` which will italicise text, or `<b></b>` which will bold the text inside the tags.
- You can use a `<div>` tag to create blocks of HTML that would otherwise exsist outside of a block and fall inlime with other page content.
- the `<span>` tag works the same as div, but for inline content.
- An Iframe is a window inside your webpage that displays another page. I.E. the map content inside google.maps.
- `<meta>` Tags contain information about the webpage that is not visiable to the browser, this will generally contain information like who made the webpage, and more.
- escape characters are needed to disply certain special characters through HTML such as <, >, or the copywrite sign.

### **Chapter 17: "HTML 5 Layout"**

- New HTML5 elements are used to identify different parts of a webpage and indicate its purpose. Or help with overall page structure.
- These new elements can produce a much cleaner overall HTML code file.
- Older browsers will not understand these elements
- To make HTML5 elements work in IE8(or older) extra JS code is required, which can be had for free from google.

### **Chapter 18: "Process & Design"**

- When making a new webpage consider who the site is for, design the webpage for that target audience, not for yourself.
- Understand why people would be visiting your webpage and what they are attempting to acheive or get from it.
- Its good to design a basic Sitemap/flowchart to denote the structure of the pages of your website.
- Use contrast and Styling to draw visitors to the essential information on your webpage. Understand that most readers will only skim page content.

## ***Js & Jquery by Jon Duckett***

### **Introduction**

- JS is used to make a webpage more interesting/dynamic/interactive, It can change how a page is displayed based on a user action. Or call a certain function to display new information if a user is to for example click on an image.

### **Chapter 1: "The ABC of Programming"**

- A script can simply be defined as series of instructions created to accomplish a goal.
- In order to efficently create a script it is important to break it into steps.

 1. Define the goal: understand what the script should accomplish or return.
 2. Design the script: split the script into a series of tasks that will accomplish your final goal
 3. Code each step: Now that you`ve broken the script into peices, you can program each small section.

- A flowchart or other visual organizational aid, can be very helpful when designing a script.
- JS is an object oriented language, Objects within your JS code can contain individual properties. Which themselfs can be further modified, as a user interacts with a page, or as functions are called and exicuted by your code.
- Methods denote how people or otherwise will interact with these objects. And what that should do when it happens. For example
    A Hotel *(object)* needs to check people in *(method)*.
    Checking people in means (steps the method takes)
     1. Answering the phone
     2. Checking for available rooms
     3. taking payment
     4. Sending confirmation

- Once the *Method* is completed the Hotel object might change to (booked) which may change what happens the next time the Check people in Method is called.
- writing a beautiful funcitonal webpage requires multiple steps.
    1. HTML Design the content of the webpage
    2. CSS Style the webpage content with rules
    3. JS Make the website more dynamic or interactive, or simply style the page further passed CSS.

- Linking a JS script to HTML requires use of the `<script></script>` tags, wherein you would place your JS code, Or better yet the file containing your JS code within the script tags.
