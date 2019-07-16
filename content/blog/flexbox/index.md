---
title: Flexbox
date: "2015-02-03T22:40:32.169Z"
description: In this post I’m going to write about flexbox and it’s properties.
---
flexbox is one of the most powerful layout system in css,which works in 1-Dimension either through main axis or cross axis. According to the requirements we can positioned and resized the small building blocks ,which made through flex on our website.It is one of the easiest way to made re-
sponsive website and adapt well to all screen sizes by using flex properties.
([Medium Link](https://medium.com/@psubham94/flexbox-35ee27c18e83))

# Flexbox Properties

## 1.Flex-wrap

Flex-wrap properties applied on parent container that defines whether the flex 
items(the items lies in container) are forced in a single line or can be flowed
into multiple lines. 

- Flex-wrap accepts three different values:
  -  ``` css
   flex-wrap: no-wrap
   ```
  -    ``` css
  flex-wrap: wrap
  ```
  -    ``` css 
  flex-wrap: wrap-reverse
  ```

>  flex-wrap: no-wrap
  > default value of flex-wrap , single line.

>   flex-wrap: wrap
  > when we have need to merge multi lines into a single lines then it is used,
    >but before it applied we have to define flex-direction.

>  flex-wrap: wrap-reverse
    > it is similar to wrap but it works in opposite direction.
### Example:-
``` html
  <div class="container">
    <div class="box">1</div>
    <div class="box">2</div>
    <div class="box">3</div>
    <div class="box">4</div>
  </div>
  <style>
    .container {
      display: flex ;
      flex-wrap: no-wrap; {result show in red}
      flex-wrap: wrap; {result show in yellow}
      flex-wrap: wrap-reverse; { result show in blue }
    }
    .box {
      width: 200px;
      height:-200px;
      Color: red/yellow/blue;
    }
  </style>
```



## 2.Flex-direction

Flex-direction is another properties of flexbox which defines the direction of flex items inside the ```<div>```. It sets how the flex items are placed within a flex container.
 - Flex-direction accepts four values row || column || row-reverse || column-reverse.

> flex-direction: rows 
 - it sets the flex items in horizontal axis oriented from left to right.


> flex-direction:row-reverse
  - it sets the flex items in horizontal axis oriented from right to left .
> flex-direction:column 
  - it sets the flex items in verticle axis oriented from top to bottom.
> flex-direction:column-reverse 
  - it sets the flex items in horizontal axis oriented from bottom to top.


## 3.Flex-flow

Flex-flow is the shorthand properties of flex-wrap and flex-direction.it’s default value is row no-wrap.
``` css
  <style>
  .container {
  flex-flow: <‘flex-direction’> || <‘flex-wrap’>
  }
  </style>
```



## 4. JUSTIFY-CONTENT

It defines how the browser distributes space between and around content items along the main-axis of a flex container. It helps distribute extra free space leftover when either all the flex items on a line.
``` css
  <style>
  .Container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
  }
  </style>
```
◆ flex-start: 
  default value of justify-content ,in which flex items are encapsuled towards the start line.
  In another words we can say that “flex-start means flex-items are aligned to the start of main axis.”



◆ flex-end: 
  opposite to flex-start.
 “flex-end means flex-items are aligned to the end of main axis.”

◆ center:
  flex items are centered along the main line/horizontal axis.

◆ space-between:
  In which the flex items are distributed in main line ,for example: if there are two flex items then
  the first item placed on start of line and the other item is placed end of the line. And if there is
  more than two items then first item placed on start of line and the last item is placed end of the 
  line and left items is placed in between even spaces.

◆ space-around :
  In which flex-Items are positioned with space before, between, and after the lines.

◆ space-evenly :
The empty space before the first and after the last item equals half of the space between each pair of adjacent items.

>  [See Complete Post on Medium](https://medium.com/@psubham94/flexbox-35ee27c18e83)



