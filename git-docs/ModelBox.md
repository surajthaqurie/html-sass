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
### 1. The Box Model

In CSS, the term "box model" is used when talking about design and layout.

The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:

![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/The%20Model%20box.png "the box model image")

###### Here,
``` 
Total Width = Right Broder + Right Padding + Specified Width + Left Broder + Left Padding; 
Total Height = Top Broder + Top Padding + Specified Height + Bottom Broder + Bottom Padding;
``` 

### 1.1 Box Types

The CSS box model describes the rectangular boxes that are generated for elements in the document tree and laid out according to the visual formatting model.The image below illustrates the types of boxes and their properties:

![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Box%20Types.png)

***a) Block-level boxes***:
- Vertically one after another (top to bottom)
- 100% of parents width

***b) Inline-level boxes***:
- Content is distributed in lines
- Occupies only content spaces
- No height and width
- Paddings and margins only horizonal (left to right)

***c) Inline-level boxes***:
- A mix of block and inline
- Occupies only content spaces
- Box model applies as showed

### 1.2 Positioning Schemas

The CSS layout algorithms, by default, size and position boxes in relation to each other so that nothing overlaps.

This specification defines several ways to violate these assumptions when needed, moving elements around in ways that can make them overlap other content:

![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Position%20Schemes.png)

***a) Normal Positioning***:
- The element are simply laid out on the page in a natural order in the code

***b) Floats Positioning***:
- Until it touches the edge of its containing box

***c) Absolute Positioning***:
- Can overlap other element occupying the same space

### 1.3 Stacking Contexts

The stacking context is a three-dimensional conceptualization of HTML elements along an imaginary z-axis relative to the user, who is assumed to be facing the viewport or the webpage. HTML elements occupy this space in priority order based on element attributes.

 The hierarchy of stacking contexts is a subset of the hierarchy of HTML elements (its siblings) because only certain elements create stacking contexts. We can say that elements that do not create their own stacking contexts are assimilated by the parent stacking context.
 
 ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Stacking%20Contexts.png)
 
 
- Same spacing occupying 
- Also handled by `Opacity` 

### 1.4. Box Sizing

By default in the CSS box model, the width and height you assign to an element is applied only to the element's content box `box-sizing: content-box;`. If the element has any border or padding, this is then added to the width and height to arrive at the size of the box that's rendered on the screen. For example, if you have four boxes with width: 25%;, if any has left or right padding or a left or right border, they will not by default fit on one line within the constraints of the parent container.

The `box-sizing: border-box;` property can be used to adjust this behavior:

`border-box` tells the browser to account for any border and padding in the values you specify for an element's width and height. If you set an element's width to 100 pixels, that 100 pixels will include any border or padding you added, and the content box will shrink to absorb that extra width. This typically makes it much easier to size elements. 

![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Boder%20Box.png)


###### Here,
``` 
Total Width = Specified Width; 
Total Height = Specified Height;
``` 
---

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
   
### [6. Layout Types](Layouts.md)
  
  This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
  
  Some imporatant layout are: ([... See more](Layouts.md))
  
### [7. Break Points](BreakPoints.md)
  
 CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

CSS breakpoints are also called media query breakpoints, as they are used with media query. ([... See more](BreakPoints.md))

---
  
All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.



