class-12.md

## **Table Of Contents**

_Read:12_

Reading
Assorted bits of documentation:

[Read this article on the Chart.js API.](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

[Chart.js docs: You’ll be needing these!](https://www.chartjs.org/docs/latest/)

Read the following articles on the Canvas API.

[Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
[Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
[Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
[Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)
  


## **Chart.js API**

- A tool enabling the easy creation of animated data visualizations in JS
- chart.js uses the html `<canvas>` tags to create beautiful charts.
- to use chart.js you need to download Chart.min.js and place it in the dir of your project, Than call it with `<script>` tags in your html
- this API makes it super easy to create great vis's with a few simple lines of JS and CSS for styling. 

## **Basic use of the Canvas HTML element**

- `<canvas>` takes in a width and height value, which can be set within the tag, or by DOM properties. 
- canvas can be styled with CSS just like any normal element, however certain rules do not effect the drawing on the canvas
- canvas creates a fixed size drawing surface. 

## **Drawing shapes with Canvas**

- canvas only supports two primitive shapes. rectangles and paths. ALl other shapes must be created by combining paths. 
- a path is a list of points connected by segments. You can control these segments as lines, or curves as well as width and color.
    1. create your path
    2. use drawing commands to draw into the path
    3. once the path is created you can stroke or fill the path to render

## **Applying styles and colors**

- To apply color to the shapes from a canvas you can use `fillStyle` and `strokeStyle` using standard CSS color methods
- there are many styles and design controls you can apply to the paths, like `round bevel miter`

## **Drawing text**

- You can draw text into a canvas with `fillText or strokeText` methods. 
- which can then be styled and positioned within the canvas using normal styling you are familiar with.
