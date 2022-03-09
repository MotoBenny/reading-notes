Class-08.md

## **Table Of Contents**

_Read:08_   More CSS Layout

## ***Ducket HTML***

1. [Learn CSS - Layout](https://web.dev/learn/css/layout/)
2. Duckett HTML/CSS book: Ch. 15, “Layout” (again; repeat of Class 4 reading)

## **Learn CSS - Layout**

- Early webpages were styled entirely with HTML tables.
- `display` property starts out by determining if the box it is applied to is inline or block-line
- you cannot set a width or height on an inline element
- [block image](https://web-dev.imgix.net/image/VbAJIREinuYvovrBzzvEyZOpw5w1/GezxDZXkJgkMevkKg39M.png?auto=format&w=1600)
- flexbox and grid are the two main design elements within CSS
- you can use floats to wrap text around an image.

### **Chapter 15: "Layout"**

- CSS treats all HTML elements as either block level or inline. Block level elements start on a new line, Inline elements flow in between text
- relative positioning moves and element in relation to where it would have been in normal flow.
- when and element is given absolute positioning the box is taken out of normal flow and no longer affects other elements.
- z-index allows you to control which elements are closer to the front of the page. or stacked on top of other elements.
- float is a great way to position elements side by side.
- clear or clearing elements ensures that no elements will touch the sides of a box.
- using float:left or float:right in conjunction with classes is a great way to create multi column layouts with elements side by side
- fixed width layouts allow finer design control, but can create sparse pages on large high resolution displays or force a webpage to look very small, or have large black margins.
- liquid layouts stretch and contract as the browser window expands or contracts. 
- a good rule of thumb for hte body element in a liquid layout is to set the width to 90%. this will ensure there is always a reasonable margin to the webpage. - see page 386 of HTML book for more details on liquid layout in practice. 
- layout grids are a good way to achieve consistent layout on a webpage. Think the rule of thirds but for website design.
- CSS frameworks contain the code for common tasks, like creating layout grids, styling forms, and so on. Utilize them in design.
- See [blueprintcss.org](blueprintcss.org) or [;essframework.com](lessframework.com) or many others for frameworks.
