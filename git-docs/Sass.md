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

---
### 4. SASS (Syntactically Awesome Stylesheet)

Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language. We need Sass compiler that converts Sass source code to Css code. 
In this project Sass syntax is used.

When stylesheets are larger, more complex, and harder to maintain then CSS pre-processor SASS can be used. SASS lets you use features that do not exist in CSS, like variables, nested rules, mixins, imports, inheritance, built-in functions, and other stuff.

#### 4.1 Sass Syntax

Sass supports two syntaxes:
  
  ***a) Sass Syntax (Indented syntax)***:
  
 Indented syntax is the older syntax and called as Sass. You have to write CSS concisely for using this type of syntax. It uses the extension .sass".
 
 It was designed and written by Ruby developers so, Sass stylesheets use Ruby like syntax with no braces, no semi-colons and a strict indentation. In Sass, the variable sign is ! instead of $ and assignment sign is = instead of :.
  
  ***b) SCSS Syntax (Sassy CSS)***:
  
 The SCSS (Sassy CSS) can be specified as an extension of CSS syntax. It simply means that every valid CSS is a valid SCSS also. SCSS makes it easy to maintain large style sheets. It uses the extension ".scss".
 
 SCSS provides the CSS friendly syntax to closing the gap between Sass and CSS. SCSS is called Sassy CSS.
 
The image below illustrates the exmaple of sass and scss syntax:
 ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Sass%20Syntax.png)
 
#### 4.2 The Main Features Of SASS

It allows you to write DRY(Don’t Repeat Yourself) code so that the code will be faster, more efficient, and easier to maintain. The main features of sass are as follows: 

The image below illustrates features of sass:
 ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/Sass%20Features.png)

***a) Varibles***:

- Resuable values such as: (font-size, color).

```
/* define primary colors */
$primary_1: #a2b9bc;
$primary_2: #b2ad7f;

/* use the variables */
.main-header {
  background-color: $primary_1; // here you can put an inline comment
}

```
***b) Nesting***:

- Selector inside of one another.
```
/* SCSS Syntax:*/
.header {
  width: 100%;
  ul{
    padding:30px;
    li{
      font-size:25px;
      &.first{
        color:green;
        font-weight:bold;
      }
      &.sec{
        color:blue;
      }
    }
  }
}

/* CSS Syntac */
.header {
  width: 100%;
}
.header ul {
  padding: 30px;
}
.header ul li {
  font-size: 25px;
}
.header ul li.first {
  color: green;
  font-weight: bold;
}
.header ul li.sec {
  color: blue;
}


```

***c) Operators***:

- For perform mathematical operation as well as condition operation.

There are diffrent type of operators:
- Assignment Operator (:)
- Arithmetic Operators (+, -, *, /, %)
- Equality Operator (==, !=)
- Comparison Operator (<, <=, >, >=) 
- Logical Operators  (AND, OR, NOT)
 

```

/* SCSS Syntax:*/
$size: 25px;

h2{
   font-size: $size + 5;
}

h3{
   font-size: $size / 5;
}

.para1 {
   font-size: $size * 1.5;
}

.para2 {
   font-size: $size - 10;
}

/* Compiled CSS Syntax */
h2 {
   font-size: 30px;
}

h3 {
   font-size: 5px;
}

.para1 {
   font-size: 37.5px;
}

.para2 {
  font-size: 15px;
}
```

***d) Partials and Import***:

- Partials are small files of Sass snippets. The underscore indicates that the file is a partial and it should not be compiled to CSS. The purpose of partials is to avoid having one extremely large CSS file with all of the app’s styling. This can get difficult to read through and maintain.
- And @imprort is used for importing these different (partials) files in the main.scss file.

```
/* Sass Import Syntax: */
@import filename;

/* SCSS Syntax (_base.scss): */

html,
body,
ul,
ol {
  margin: 0;
  padding: 0;
}

/* SCSS Syntax (main.scss): */
@import "base/base";

body {
  font-family: Helvetica, sans-serif;
  font-size: 18px;
  color: red;
}

/* CSS output: */

html, body, ul, ol {
  margin: 0;
  padding: 0;
}

body {
  font-family: Helvetica, sans-serif;
  font-size: 18px;
  color: red;
}

```

***e) Mixins***:

- Reusable pieces.
- The @mixin directive lets you create CSS code that is to be reused throughout the website.
- The @include directive is created to let you use (include) the mixin.

```
/* Defining a Mixin SCSS Syntax:*/

/* Variables: define primary colors */
$primary_1: #a2b9bc;


@mixin important-text {
  font-size: 25px;
 }

@mixin colorfix($color){
color: $color;
}


/*Using a Mixin SCSS Syntax:*/

.danger {
  @include important-text;
  @include colorfix($primary_1);
  background-color: green;
  border: 1px solid blue;

}

/* CSS output: */
.danger {
  color: #a2b9bc;
  font-size: 25px;
  border: 1px solid blue;
  background-color: green;
}
```

***f) Function***:

- produce value that can be used.

In Sass we can use two type of function. They are:

a) Inbuilt Function:

```
/* Variables: define primary colors */
$primary_1: #a2b9bc;

nav{
darker($primary_1, 15%);
lighten($primary_1, 15%);
}
```

b) User-define function:

```
@function divide($a, $b)
  @return $a/$b;
  
  nav{
    margin: divide (60, 2) * 1px;  // * 1px -> convert to pixel
  }

```

***g) Extends***:

- Inherit decelaration (work as parent element).
- These are written in %name and than @extend name;

```
/*Using a Extends SCSS Syntax:*/

/* Variables: define primary colors */
$primary_1: #a2b9bc;
$primary_2: #b2ad7f;

// Inherit decelaration
%btn-placholder{
padding: 10px;
display: inline-block;
text-aling: center;
}

// use of extends
.btn-main{
 &:link{
  @extend %btn-placeholder;
  background: $primary_1;
  }
}

.btn-hot{
 &:link{
  @extend %btn-placeholder;
  background: $primary_2;
  }
}

/* CSS output: */

.btn-main:link, .btn-hot:link{
     padding: 10px;
     display: inline-block;
     text-aling: center;
  }

.btn-main:link{
    background: $a2b9bc;
  }
  
 btn-hot:link{
    background: $b2ad7f;
  }

```

***h) Control Directives***:

- Conditonal and loops.

```
Example of For loop:

@mixin respond($breakpoint) {
    @if $breakpoint == phone {
      // Media qurey only applied to the screens eg: print out our page these medai query donot apply
    @media only screen and (max-width: 37.5em) { @content }; // 600px (600/16)
  }
  @if $breakpoint == tab-port {
    @media only screen and (max-width: 56.25em) { @content }; // 900px
  }
  @if $breakpoint == tab-land {
    @media only screen and (max-width: 75em) { @content }; // 1200px
  }
  @if $breakpoint == big-desktop {
    @media only screen and (min-width: 112.5em) { @content }; // 1800px
  }
}

```
#### 4.3 BEM (Block Element Modifier) Selectors

BEM is a method on how HTML element classes should be named. BEM class names are meant to be straightforward and self-explanatory. Class names are formatted as: block__element--modifier (block double underscore element double dash modifier).

```
Let’s look at this example:

<nav className="nav">
<h1 className="nav__h1">Big Cat Refuge</h1>
<ul className="nav__ul">
<li className="nav__li">Home</li>
<li className="nav__li">About</li>
<li className="nav__li">Contact</li>
</ul>
<button className="nav__btn--hover">Change Theme</button>
</nav>
```
 ![alt text](https://github.com/surajthaqurie/html-sass/blob/master/git-docs/images/BEM%20Classname.png)


#### 4.4 Architecting With Files And Folder

One of the popular way to structure Sass apps is to use the 7–1 architecture. The 7–1 pattern indicates that we create 7 folders and 1 main Sass file where we import all the files from these 7 folders. This technique is usually used for large projects with multiple pages. Take a look at this example structure:

```
Sass/
|
|– abstracts/
|   |– _variables.scss    # Sass Variables
|   |– _mixins.scss       # Sass Mixins
|   |– _functions.scss    # Sass Functions
|
|– vendors/
|   |– _icons.scss        # Font-Awesome Icons
|
|– base/
|   |– _reset.scss        # Reset
|   |– _typography.scss   # Typography rules
|   |– _animations.scss   # Animation rules
|   |– _utilities.scss    # Utility rules
|
|– layout/
|   |– _navigation.scss   # Navigation
|   |– _header.scss       # Header
|   |– _footer.scss       # Footer
|
|– components/
|   |– _buttons.scss      # Buttons
|   |– _card.scss         # Card
|   |– _form.scss         # Form
|
|– pages/
|   |– _home.scss         # Home page style
|   |– _contact.scss      # Contact page style
|   |– _about.scss        # About page style
|
|– themes/
|   |– _pink.scss         # Pink theme
|   |– _mint.scss         # Mint theme
|
 – main.scss              # Main Sass input file
 ```

```
- base/ : basic project definitions.
- components/: resuable building blocks.
- layouts/: global layouts of entire project.
- pages/: specific pages of entire project.
- themes/: different themes of project.
- abstracts/: variables, mixins and other stuff.
- vendors/: third party css eg. bootstrap, icon system
```
##### main.scss

In the main.scss file, we import all the partials. Order matters. The order of your imports is the order Sass will follow during processing. The general rule is to have all the “logic” files (mixins, variables, functions) at the top. The main.scss file should look like this:

```
@import 'abstracts/variables';
@import 'abstracts/mixins';
@import 'abstracts/functions';
@import 'vendors/icons';

//etc..
```

``` NOTE: The sass-compiler compiles the main.scss file into css file. ```

---
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
