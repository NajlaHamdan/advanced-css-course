# different between css variable and sass variable

#### css variable

- custome property in css
- does not need to preprocessor
- we can manipulate it with javaScript
- can be inherited
- defiend within declaration block {} and usually we but it in root selector
- can not used with media query .

# flexbox properties

### properties in container

- flex-direction:row;
  meaning:
  values: row,row-reverse,column,column-reverse.
  default value: row.
- justify-content:flex-start;
  meaning:
  values :
  default value:
- align-items:baseline;
  meaning:
  values :
  default value:
- flex-wrap:wrap;
  meaning:
  values :
  default value:
- align-content:center;
  meaning:
  values :
  default value:

### properties in items

- align-self:flex-start;
  like align content but used to spacify alignment to one item
- order:-1;
  used to order the items
  default number for all items is 0 that mean positive values will be at the end and negative at the start.
- flex-grow:0;
  has two values 0 -> not allowed to grow 1-> allowed to grow
- flex-shrink:0;
  has two values 0 -> not allowed to shrink 1-> allowed to shrink
- flex-basis
  used to spacify width of the flex item
- flex:
  shortcut for flex grow , shrink and basis

  # different between icon fonts and SVG
  icon fonts problem
  - in fact it just a hack to display icons which are like images using a font .
  - icon fonts fail more than you think and in that case the browser will displays a blank square .
  - screenreaders for blind people try to read icon font and of course fail to read icon font
better alternative for icon fonts is SVG
  SVG stands for scalable vector graphics
  SVG is just a way to writing a vector graphics with code .
   resourse to find , generate and convert icon font to  SVGs is icomoon.io .

   -- the goal of having one sprite img file is to have one http request


### box-sizing 
- content-box
default value 
padding , margin and border will added to width and height of the content
padding , margin and border are not included in width and height of the content
-- because that element often appears bigger than you have set (because the element's border and padding are added to the element's specified width/height).
width + padding + border = actual width of an element
height + padding + border = actual height of an element
- border-box
padding , margin and border are included in width and height of the content
because that the element does not become bigger than the width and hieght when you add padding , margin or border.

### z-index
does not work without position property


### differences between px,rem and em
https://zellwk.com/blog/media-query-units/