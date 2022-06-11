# This is my journal 6/11/2022

## What I have learned today

-Today I learned about the canvas feature in HTML

- <Canvas> requires at least two other attributes. Height and width.

- It allows you to draw 2D graphics with javascript.

- You can access it's properties with the canvas.width and the canvas.height.

- Canvas requires a closing tag. It is also blank by default.

- Canvas has the feature getContext() which is a method that takes one argument. Using the 2D to get a 2d rendering context object.

> Example: let canvas = document.querySelector('#canvas');
> let ctx = main.getContext('2d');

> let canvas = document.querySelector('#main');
> if(canvas.getContext) {
> let ctx = main.getContext('2d');
> }(www.javascripttutorial.net/web-apis/javascript-canvas/)

- The previous line of code is used to check to see if the browser can use the getContext() method.

- The 2d drawing method features simple drawing methods for making simple shapes like squares, triangles and rectangles.

> All coordinate values are calculated in relation to the (0,0) with x increasing to the right and y increasing to the bottom. (www.javascripttutorial.net/web-apis/javascript-canvas/)

- The fillStyle and strokeStyle properties of the 2D drawing context will determine the fill and stroke styles.


