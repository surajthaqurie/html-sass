  # Html Css with Sass

  Simple over view of Html Css with Sass(syntactically awesome style sheets).

  In this repository basically there are four projects and they builds in different  Css layout:
  - ***Natours*** :```Float Layout```
  - ***Trillo*** :```Flexbox Layout```
  - ***Nexter*** :```Grid Layout```
  - ***Omnifood*** :```Grid and Flexbox Layout but without SASS```

  ## Install Sass

  You can install Sass on Windows, Mac, or Linux by downloading the package for
  your operating system [from GitHub][] and [adding it to your `PATH`][PATH].
  That's all—there are no external dependencies and nothing else you need to
  install.

  [from GitHub]: https://github.com/sass/dart-sass/releases
  [PATH]: https://katiek2.github.io/path-doc/

  In this project we use ```node-sass``` package. If you use Node.js, you can also install Sass using [npm][] by running.

  [npm]: https://www.npmjs.com/

  ```
  npm install node-sass --save-dev
  ```

  Once you have node-sass installed, you have to add script for sass compiler in package.json file. For example
  ```
  "script:{
  "compile:sass": "node-sass sass/main.scss css/style.css",
  }
  ```
  To run above script compile:sass, In terminal type ```npm run compile:sass``` and hit enter.

  **Some IMP Stuffs:**

  ***```"watch:sass": "node-sass sass/main.scss css/style.css -w"```***: 
  - This script watches the changes and automatically save the new changes.
    
  ***```"concat:css": "concat -o css/style.concat.css css/icon-font-styles.css css/style.comp.css"```***: 
  - This script concates the two files into one.
  - For run this we have to install ```concat``` package  by using npm. 
  - To install ```npm install concat --save-dev```. 
  - To run above script "concat:sass", In terminal type ```npm run compile:sass``` and hit enter.
      
  ***```"prefix:css": "postcss --use autoprefixer -b 'last 10 versions' css/style.concat.css -o css/style.prefix.css"```***:
  - This script prefix the css automatically which are supported in different browser with different version. Here 10 last versions.
  -  For run this, we have to install ```postcss``` and ```autoprefixer``` packages  by using npm.
  -  To install ```npm install postcss autoprefixer --save-dev```. 
  -  To run above script "prefix:sass", In terminal type ```npm run prefix:sass``` and hit enter.
      
  ***```"compress:css": "node-sass css/style.prefix.css css/style.min.css --output-style compressed"```***: 
  - This script compressed the css file. 
  - To run above script "compress:sass", In terminal type ```npm run compress:sass``` and hit enter.
      
      
  ***```"build:css": "npm-run-all  compile:sass concat:css prefix:css compress:css"```***:
  - This script runs all the script one by one automatically.
  - For run this, we have to install ```npm-run-all``` package by using npm. 
  - To install ```npm install npm-run-all --save-dev```. 
  - To run above script "build:sass", In terminal type ```npm run build:sass``` and hit enter. 


  ```NOTE: We can also use other compiler: For Example```
  ```
  npm install -g sass
  ```

  To compile sass file in to css file, in the terminal type:

  ```
  sass source/stylesheets/index.scss build/stylesheets/index.css
  ```
  ---

  ## Hot topics of the project

  In this project their are different topics are discussed. Some important topics are as follows:

  ### [1. The Box Model](git-docs/ModelBox.md)

  In CSS, the term "box model" is used when talking about design and layout.

  The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. ([... See more](git-docs/ModelBox.md))

  ### [2. CSS Behind The Scenes](git-docs/BehindTheScenes.md)

  Before jumping right into the topic, we have to look at the first thing that happens while loading a website in a browser. When the root HTML document is being loaded, that is what we call being parsed.

  After Loading HTML then, file two process are occurs: ([...See more](git-docs/BehindTheScenes.md))

  ### [3. Values In CSS](git-docs/ValuseInCss.md)

  Every CSS declaration includes a property / value pair. Depending on the property, the value can include a single integer or keyword, to a series of keywords and values with or without units.

  In this sections we discussed about: ([...See more](git-docs/ValuseInCss.md))

  ### [4. SASS (Syntactically Awesome Stylesheet)](git-docs/Sass.md)

  Sass is a CSS preprocessor, an extension of CSS that adds power and elegance to the basic language. We need Sass compiler that converts Sass source code to Css code. 

  In this sections we discussed about: ([...See more](git-docs/Sass.md))

  ### [5. Responsive Design](git-docs/Responsive.md)

  Responsive Web design is the approach that suggests that design and development should respond to the user’s behavior and environment based on screen size, platform and orientation.

  But responsive Web design is not only about adjustable screen resolutions and automatically resizable images, but rather about a whole new way of thinking about design.  ([... See more](git-docs/Responsive.md))
    
  ### [6. Layout Types](git-docs/Layouts.md)
    
This Section will recap some of the CSS layout features we've already touched upon in previous modules, such as different ```display``` values, as well as introduce some of the concepts we'll be covering throughout this module.
    
Some imporatant layout are: ([... See more](git-docs/Layouts.md))
    
  ### [7. Break Points](git-docs/BreakPoints.md)
    
  CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.

  CSS breakpoints are also called media query breakpoints, as they are used with media query. ([... See more](git-docs/BreakPoints.md))

  ---


All Projects Notes Images and  Documents are refrenced from

Copyright (c) Jonas Schmedtman.


