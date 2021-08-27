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


---
### 3. Values In CSS

Every CSS declaration includes a property / value pair. Depending on the property, the value can include a single integer or keyword, to a series of keywords and values with or without units.

In this sections we discussed about:

3.1 Value Processing

3.2 Value Conversion

3.3 Inheritance Value

#### 3.1 Value Processing

Once a user agent has parsed a document and constructed a document tree, it must assign, to every element in the tree, and correspondingly to every box in the formatting structure, a value to every property that applies to the target media type.

The final value of a CSS property for a given element or box is the result of a multi-step calculation. The image below illustrates the Value Processing:


![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Css%20Value%20Processing.png)



#### 3.2 Value Conversion

CSS has several different units for expressing a length.Many CSS properties take "length" values, such as width, margin, padding, font-size, border-width, etc.
Length is a number followed by a length unit, such as 10px, 2em, etc.  whitespace cannot appear between the number and the unit. However, if the value is 0, the unit can be omitted.

There are two types of length units: relative and absolute.

- ***Relative***: Relative length units specify a length relative to another length property. Relative length units scales better between different rendering mediums.

- ***Absolute***: The absolute length units are fixed and a length expressed in any of these will appear as exactly that size. Absolute length units are not recommended for use on screen, because screen sizes vary so much. However, they can be used if the output medium is known, such as for print layout.

The image below illustrates the Value Converting:

![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Css%20Value%20Conversion.png)

``` 
Some Relative units are:
a. em	Relative to the font-size of the element (2em means 2 times the size of the current font)
b. ex	Relative to the x-height of the current font (rarely used)
c. ch	Relative to width of the "0" (zero)
d. rem	Relative to font-size of the root element (by default fontsize: 16px)
e. vw	Relative to 1% of the width of the viewport*
f. vh	Relative to 1% of the height of the viewport*
g. vmin	Relative to 1% of viewport's* smaller dimension
h. vmax	Relative to 1% of viewport's* larger dimension
i. %	 

TIP: The em and rem units are practical in creating perfectly scalable layout!
   * Viewport = the browser window size. If the viewport is 50cm wide, 1vw = 0.5cm.

Some Absolute units are:
a. cm	centimeters
b. mm	millimeters
c. in	inches (1in = 96px = 2.54cm)
d. px *	pixels (1px = 1/96th of 1in)
e. pt	points (1pt = 1/72 of 1in)
f. pc	picas (1pc = 12 pt)

NOTE: * Pixels (px) are relative to the viewing device. For low-dpi devices, 1px is one device pixel (dot) of the display. For printers and high resolution screens 1px implies multiple device pixels.

```

#### 3.3 Inheritance Value

When different declarations try to set a value for the same element/property combination, the conflicts must somehow be resolved.

The opposite problem arises when no declarations try to set a the value for an element/property combination. In this case, a value is be found by way of inheritance or by looking at the property’s initial value. The image below illustrates the inheritance value:

![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Css%20Inheritance.png)

---

### [4. SASS (Syntactically Awesome Stylesheet)](Sass.md)

Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language. We need Sass compiler that converts Sass source code to Css code. 

In this sections we discussed about: ([...See more](Sass.md))

### [5. Responsive Design](Responsive.md)

Responsive Web design is the approach that suggests that design and development should respond to the user’s behavior and environment based on screen size, platform and orientation.

But responsive Web design is not only about adjustable screen resolutions and automatically resizable images, but rather about a whole new way of thinking about design.  ([... See more](Responsive.md))
   
### [6. Layout Types](Layouts.md)
  
  This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
  
  Some imporatant layout are: ([... See more](Layouts.md))
  
### [7. Break Points](BreakPoints.md)
  
 CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

CSS breakpoints are also called media query breakpoints, as they are used with media query. ([... See more](BreakPoints.md))

---

All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.







