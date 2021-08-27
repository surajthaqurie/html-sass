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

---

### 2. CSS Behind The Scenes

Before jumping right into the topic, we have to look at the first thing that happens while loading a website in a browser. When the root HTML document is being loaded, that is what we call being parsed.

After Loading HTML then, file two process are occurs:

2.1 Parse HTML

2.2 Load CSS

The image below illustrates that how browser handle tha HTML document:
 ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Css%20Behind%20The%20Scene.png)


#### 2.1 Parse HTMl

Parsing means taking the HTML code and then extracting valuable information from it. This includes information like the title of the page, header links, and the body content.

After it parses the HTML document, all it stores the code in a DOM (Document Object Model). It describes the entire web page consisting of parents, children, and siblings. It separates the header links that contain the CSS files during parsing.

#### 2.2 Load CSS

The separated CSS files go to the next step, i.e. loading the CSS files.

After loading the CSS files, the parsing of CSS occurs, similar to the parsing of the HTML files, but there’s a slight difference. The parsing of CSS files takes place in two steps, and it’s a bit more complex.4

a) Resolving the CSS declarations conflicts (Cascading)

b) Processing final CSS values.


***a) Resolving the CSS declarations conflicts (Cascading)***:

This is firts step of css parse: Resolving the CSS declarations conflicts, and this step is also known as Cascading. Sometimes, while writing CSS, some block of rules applies to certain elements, and some do not. This happens because some styles have higher importance or specificity over others.
 
 There are three kinds of CSS:
 ```
 i) Author Declarations: CSS that developers write
 ii) User Declarations: Settings created by the user in the browser, for example setting font-size in the browser
 iii) Browser Declarations: Also known as user-agent default browser declarations

```
Cascade combines the CSS declarations coming from all these different sources.

But how does the cascade actually resolve conflicts? By looking at the importance, specificity, and source order of conflicting declarations in order to determine which one takes precedence.The image below illustrates the order of how we look at the importance, specificity, and source order for all the matching rules:

 ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Css%20Priorities.png)
 
 
```
Factors such as:

- !important: defines it is important than other

- Specificity: Inline styles > IDs > Classes or Pseudo classes > elements or pseudo elements. We can find the specificity of any element based on the selectors we are using like this: (I, ID, C, E).

- Source Order: If all the declaration selectors have the same specificity, then the last declaration will be used. The last declaration in the code will overwrite all other declarations and will be applied.

```

***b) Processing final CSS values***:

This step includes giving the final processed values to all the styles. Here the values are processed and the units (rem, em,%, etc …) are converted into pixels for the correct rendering in the browser.

The values declared by the developer are at the top of the chain. These values are evaluated and passed to the next step, which are the values specified by the Cascade.

If the developer does not declare any specific value, such as font-size, the Cascade sets a default value that in most browsers is 16px.


---

### [3. Values In CSS](ValuseInCss.md)

Every CSS declaration includes a property / value pair. Depending on the property, the value can include a single integer or keyword, to a series of keywords and values with or without units.

In this sections we discussed about: ([...See more](ValuseInCss.md))

### [4. SASS (Syntactically Awesome Stylesheet)](Sass.md)

Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language. We need Sass compiler that converts Sass source code to Css code. 

In this sections we discussed about: ([...See more](Sass.md))

### [5. Responsive Design](Responsive.md)

Responsive Web design is the approach that suggests that design and development should respond to the user’s behavior and environment based on screen size, platform and orientation.

But responsive Web design is not only about adjustable screen resolutions and automatically resizable images, but rather about a whole new way of thinking about design.  ([... See more](git-Responsive.md))
   
### [6. Layout Types](Layouts.md)
  
  This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
  
  Some imporatant layout are: ([... See more](Layouts.md))
  
### [7. Break Points](BreakPoints.md)
  
 CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

CSS breakpoints are also called media query breakpoints, as they are used with media query. ([... See more](BreakPoints.md))

---

  
All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.








