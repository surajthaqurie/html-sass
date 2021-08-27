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

---
### 5. Responsive Design

Responsive Web design is the approach that suggests that design and development should respond to the user’s behavior and environment based on screen size, platform and orientation.

But responsive Web design is not only about adjustable screen resolutions and automatically resizable images, but rather about a whole new way of thinking about design. Let’s talk about all of these features, plus additional ideas in the making.

The image below illustrates the Responsive Design:
  
   ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Responsivedesign.png)
  

#### 5.1 Fluid Grid And Layouts

The layout of a website has to respond and adapt to the dimensions of the device on which it is displayed (responsive design). A fluid grid layout provides a visual way to create different layouts corresponding to devices on which the website is displayed.

For example, your website is going to be viewed on desktops, tablets, and mobile phones. You can use fluid grid layouts to specify layouts for each of these devices. Depending on whether the website is displayed on a desktop, tablet, or mobile phone, the corresponding layout is used to display the website.

- Should uses % rather then px.

#### 5.2 Flexible/ Responsive Image

***a) The flexible images***, often also called adaptive images. respond to different viewport sizes and display resolutions. It seeks to overcome two problems facing visual elements in the age of mobile development.

Making images to scale with a fluid layout can be achieved simply for modern browsers. It's as simple as declaring the following in the CSS:

```
img {

    max-width: 100%;

}
```
  
- If the width property is set to a percentage and the height property is set to "auto", the image will be responsive and scale up and down. (works as % of parent element).
- Should adapted nicely to the current viewport.

***b) Responsive Image***, it fixes, if your site is being increasingly viewed on smaller, slower, low bandwidth devices. On those devices your desktop-centric images load slowly, cause UI lag, and cost you and your visitors un-necessary bandwidth and money.

``` NOTE: In the project,the process for making responsive image are done in both html and css. ```


- If you look at the HTML source of a responsive page, you will usually see the following <meta> tag in the <head> of the document.

  ```<meta name="viewport" content="width=device-width,initial-scale=1"> ```
  
#### 5.3 Media Queries
  
  Media queries are useful when you want to modify your site or app depending on a device's general type (such as print vs. screen) or specific characteristics and parameters (such as screen resolution or browser viewport width).

Media queries are used for the following:

- To conditionally apply styles with the CSS @media and @import at-rules.
- To target specific media for the <style>, <link>, <source>, and other HTML elements with the media= attribute.
- To test and monitor media states using the Window.matchMedia() and MediaQueryList.addListener() JavaScript methods.
  
  ```NOTE: The examples on this page use CSS's @media for illustrative purposes, but the basic syntax remains the same for all types of media queries.```
  
 #### 5.4 Responsive Design Strategies
  
  There are two type of responsive design strategies:
  
  ***a)Desktop-First***:
  - Start writting Css for the desktop: large screen
  - The, media queries shrink design to smaller screens.
  
  ``` 
  Example: 
  
  html { font-size:20px; }
  @media (max-width: 600px){ 
  html { font-size: 16px; 
   }
  ```
  
  ***b)Mobile-First***:
  - Start writing CSS for mobile devices: small screen;
  - Then, media qureies expand design to a large desktop screen;
  - Forces us to reduce website and apps to the absolute essentials.

   ``` 
  Example: 
  
  html { font-size:16px; }
  @media (min-width: 600px){
  html { font-size: 20px; 
   }
  ```
  
  The image below illustrates the responsive design Strategies:
  
   ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Responsive%20Design%20Strategies.png)

  ---
  
   ### [6. Layout Types](Layouts.md)
  
  This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
  
  Some imporatant layout are: ([... See more](Layouts.md))
  
 ### [7. Break Points](BreakPoints.md)
  
 CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

CSS breakpoints are also called media query breakpoints, as they are used with media query. ([... See more](BreakPoints.md))

  ---

All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.



