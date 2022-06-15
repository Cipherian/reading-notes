# This is my journal 6/14/2022

## What I have learned today from

> (www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)

- Today I learned some more CSS effects.

- fade:hover with opacity makes it so you can see a fade in.

- color:hover makes it so it changes color when you hover over.

-grow:hover makes it so an element grows.
  -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);

- .shrink:hover makes it so an element shrinks when you hover.

{
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
}

.rotate:hover makes it so an element rotates when you hover.
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}

- .threed:hover gives your element 3d shadow.
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}

- .border:hover gives you an inset border
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}

## What I learned from

- (learn.shayhowe.com/advanced-html-css/css-transforms/)

> Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.


> It is possible to scale only the height or width of an element using the scaleX and scaleY values. The scaleX value will scale the width of an element while the scaleY value will scale the height of an element. To scale both the height and width of an element but at different sizes, the x and y axis values may be set simultaneously. To do so, use the scale transform declaring the x axis value first, followed by a comma, and then the y axis value.