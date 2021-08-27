# [Html Css with Sass](/README.md)

  Simple over view of Html Css with Sass(syntactically awesome style sheets).

## [Install Sass](/README.md)

You can install Sass on Windows, Mac, or Linux by downloading the package for
your operating system [from GitHub][] and [adding it to your `PATH`][PATH].
That's all—there are no external dependencies and nothing else you need to
install.

[from GitHub]: https://github.com/sass/dart-sass/releases
[PATH]: https://katiek2.github.io/path-doc/

## Hot topics of the project

In this project their are different topics are discussed. Some important topics are as follows:

### [1. The Box Model](ModelBox.md)

In CSS, the term "box model" is used when talking about design and layout.

The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. ([... See more](ModelBox.md))

### [2. CSS Behind The Scenes](BehindTheScenes.md)

Before jumping right into the topic, we have to look at the first thing that happens while loading a website in a browser. When the root HTML document is being loaded, that is what we call being parsed.

After Loading HTML then, file two process are occurs: ([...See more](BehindTheScenes.md))

### [3. Values In CSS](ValuseInCss.md)

Every CSS declaration includes a property / value pair. Depending on the property, the value can include a single integer or keyword, to a series of keywords and values with or without units.

In this sections we discussed about: ([...See more](ValuseInCss.md))

### [4. SASS (Syntactically Awesome Stylesheet)](Sass.md)

Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language. We need Sass compiler that converts Sass source code to Css code. 

In this sections we discussed about: ([...See more](Sass.md))

### [5. Responsive Design](Responsive.md)

Responsive Web design is the approach that suggests that design and development should respond to the user’s behavior and environment based on screen size, platform and orientation.

But responsive Web design is not only about adjustable screen resolutions and automatically resizable images, but rather about a whole new way of thinking about design.  ([... See more](Responsive.md))

---
   
 ### 6. Layout Types
  
  This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
  
  Some imporatant layout are:
  
#### 6.1 Float
  
Floating an element changes the behavior of that element and the block level elements that follow it in normal flow. The floated element is moved to the left or right and removed from normal flow, and the surrounding content floats around it.

The float property has four possible values:

- left — Floats the element to the left.
- right — Floats the element to the right.
- none — Specifies no floating at all. This is the default value.
- inherit — Specifies that the value of the float property should be inherited from the element's parent element.
  
#### 6.2 FlexBox
  
 Flexbox is the short name for the Flexible Box Layout CSS module, designed to make it easy for us to lay things out in one dimension — either as a row or as a column. To use flexbox, you apply display: flex to the parent element of the elements you want to lay out; all its direct children then become flex items. We can see this in a simple example.
  
  ```
  Syntax:
   display: flex;

  ``` 
  
#### 6.3 Grid Layout
  
 While flexbox is designed for one-dimensional layout, Grid Layout is designed for two dimensions — lining things up in rows and columns.

Similar to flexbox, we enable Grid Layout with its specific display value — display: grid.

   ```
  Syntax:
   display: grid;

  ```
  
 **And other CSS layouts are**:
- ***Normal flow***: Normal flow is how the browser lays out HTML pages by default when you do nothing to control page layout. 
- ***The display property***: Standard values such as block, inline or inline-block can change how elements behave in normal flow.
- ***Positioning***: Allows you to precisely control the placement of boxes inside other boxes. static positioning is the default in normal flow, but you can cause elements to be laid out differently using other values
- ***Table layout***: Features designed for styling parts of an HTML table can be used on non-table elements using display: table and associated properties.
- ***Multiple-column layout***: The Multi-column layout properties can cause the content of a block to layout in columns, as you might see in a newspaper.

The image below illustrates the Layouts:
  
   ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Layouts%20Types.png)
  
  ---
  
### [7. Break Points](BreakPoints.md)
  
 CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

CSS breakpoints are also called media query breakpoints, as they are used with media query. ([... See more](BreakPoints.md))


  ---

All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.



