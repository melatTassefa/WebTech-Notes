# CSS Components

# Introduction to CSS

CSS, short for Cascading Style Sheets, is a language used to style a web page. It's to be added onto HTML file to define the design and layout of the web page. Listed below are some of the components of CSS:

## CSS Selectors

CSS selectors are used to specify a certain HTML tag to style. Some of the basic CSS selectors are:

### The CSS element Selector

It selects based on the element name. Example: a heading with tag <h1> is selected in CSS as follows: 

```css
h1 {
color: red;
}
```

### The CSS id Selector

It’s used to select an HTML element with a specified id. Example: a heading with id head1, <h1 id=”head1”> is referenced in CSS as follows:

```css
#head1 {
color: red;
}
```

### The CSS class Selector

It’s used to select an HTML element with a specified class name. Example: a heading with class ch1, <h1 class=”ch1”> is referenced in CSS as follows:

```css
.ch1 {
color: red
}
```

### The CSS Universal Selector

It selects all HTML elements on the page. The following code aligns all texts in the web page at the center.

```css
* {
text-align: center;
}
```

### The CSS Grouping Selector

It’s used to select more than one HTML elements which are to be given the same style. In the code below, heading 1 and 2 are both to be blue and aligned left.

```css
h1, h2 {
color: blue;
text-align: left;
}
```

## CSS Margins

CSS Margins are used to define the space around elements. They’re completely transparent. margin-top, margin-right, margin-bottom, and margin-left are used to specify the margin for their respective sides.

The values of the margin properties are the following:

- auto: margin calculated by browser
- length: requires a specific margin in px, cm, etc.
- %: requires a specific % of the width of the containing element
- inherit: specifies that the margin is to be inherited from the parent element.

```css
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```

## CSS Padding

CSS Padding is used to define the space between an element’s content and its border.

CSS has properties for specifying the padding for each side of an element:

- padding-top
- padding-right
- padding-bottom
- padding-left

All the padding properties can have the following values:

- length - specifies a padding in px, cm, etc.
- *%* - specifies a padding in % of the width of the containing element
- inherit - specifies that the padding should be inherited from the parent element

For both Margin and Padding, there’s a shorthand representation to define all four sides in one line in the order, top, right, bottom, left.

```css
div {
  padding: 25px 50px 75px 100px;
}
```

## CSS Links

CSS helps to style links in different ways. One way is to style them based on the state they are in, which is listed as follows:

- a:link - unvisited link
- a:visited - visited link
- a:hover - a link being hovered upon
- a:active - a link, the moment it’s clicked

When setting the style for several link states, there are some order rules:

- a:hover MUST come after a:link and a:visited
- a:active MUST come after a:hover

There are also other CSS properties like text-decoration and background-color to style a link.

```css
a:link {
  color: red;
}

a:visited {
  color: green;
}

a:hover {
  color: hotpink;
}

a:active {
  color: blue;
}
```

## CSS Position

The position property specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky). Based on these properties, elements are positioned with the top, bottom, left and right properties.

- static: specifies the element to be positioned according to the normal flow of the page. It’s not altered by the top, bottom, left, or right properties.
- relative: positions an element relative to its normal position. Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position.
- fixed: positions an element relative to the viewport, making it stay in the same place even if the page is scrolled.
- absolute: positions an element relative to the nearest positioned element.
- sticky: toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it becomes fixed.

## The Z-index Property

It specifies the stack order of an element (which element should be placed in front of, or behind, the others). An element can have a positive or negative z-index. An element with greater stack order is always above an element with a lower stack order.

## CSS Overflow

CSS Overflow controls what happens to content that is too big to fit into an area. It has the following values:

- visible - Default. The overflow is not clipped. The content renders outside the element's box.
- hidden - The overflow is clipped, and the rest of the content will be invisible.
- scroll - The overflow is clipped, and a scrollbar is added to see the rest of the content.
- auto - similar to scroll, but it adds scrollbars only when necessary.

### overflow-x and overflow-y

They specify whether to change the overflow of content just horizontally or vertically (or both).

## CSS Dropdown

It’s used create a dropdown activated when it’s hovered upon. 

**HTML)** Use any element to open the dropdown content, e.g. a <span>, or a <button> element.

Use a container element (like <div>) to create the dropdown content and add whatever you want inside of it.

Wrap a <div> element around the elements to position the dropdown content correctly with CSS.

**CSS)** The dropdown class uses position: relative;, which is needed when we want the dropdown content to be placed right below the dropdown button (using position: absolute;).

## CSS Rounded Corners

In order to give any element rounded corners, use the border-radius property. This property defines the radius of an element's corners.

```css
#rcorners1 {
  border-radius: 25px;
  background: #73AD21;
  padding: 20px;
  width: 200px;
  height: 150px;
}
```

The  border-radius property can have from one to four values. Here are the rules:

- **Four values - border-radius: 15px 50px 30px 5px;** (first value applies to top-left corner, second value applies to top-right corner, third value applies to bottom-right corner, and fourth value applies to bottom-left corner)
- **Three values - border-radius: 15px 50px 30px;** (first value applies to top-left corner, second value applies to top-right and bottom-left corners, and third value applies to bottom-right corner):
- **Two values - border-radius: 15px 50px;** (first value applies to top-left and bottom-right corners, and the second value applies to top-right and bottom-left corners):
- **One value - border-radius: 15px;** (the value applies to all four corners, which are rounded equally:

## CSS Buttons

background-color, font-size, padding, border-radius, width and border are used to style a button.

The :hover property is used to change the style of a button when you move the mouse over it. And the transition-duration property determines the speed of the “hover” effect.

The box-shadow property, which takes 4 values, adds shadows to a button.
