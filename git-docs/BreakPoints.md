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
   
### [6. Layout Types](Layouts.md)
  
  This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
  
  Some imporatant layout are: ([... See more](Layouts.md))

  ---
    
  ### 7. Break Points
  
 CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

CSS breakpoints are also called media query breakpoints, as they are used with media query.
  
The tricky part is to decide the breakpoints themselves. There aren’t any standard templates, and different frameworks use different breakpoints. There are three probable ways for selecting the breakpoints: The Options
  
 - ***The Bad***: It consists of simply using the width of popular devices as tha breakpoints: (like iphone and the iPad, to set breakpoints for there screen width).
  - ***The Good***: In the good way, we look at all the most-used device width on the entire internet, try to group them together in a logical way and then pick our break points from that.
  - ***The Prefect***: It is to ignore devices all together and only look at your content and your design. So, ideally, it works likes this. You begin at one size, either mobile or desktop and then start increasing your screen width or decreasing for desktop first. Then, as soon as the design breaks, it no longer looks okay, then you insert a new brekpoint. 

The image below illustrates the ways of selecting the breakpoints:
  
![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Selecting%20Breakpoint.png)
  

  In this project the good way approach is used:
  We start most-used screen size, that we can get from an app (StatCounter).

  The image below illustrates the good ways of selecting the breakpoints:
  
  ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Good%20BreakPoint.png)
  

```NOTE: Order** - Always larger breakpoint condition before smaller one.```

---

All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.



