## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed!
In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

My submission can be found on GitHub at http://FlyingBiker.github.io

To get the PageSpeed above 90 on index.html:
- Index.html
  - Removed googleapis and placed font face found at the google site into style.css
  - Inlined header p, header p span and li p styles
  - Added mdeia="print" to css/print/css link
  - Moved links to css to end of html
  - Added async to google-analytics script entry
  - Resized and compressed pizzeria.jpg and profilepic.jpeg using jpeg-optimizer that I found online

To get 60 fps pizza.html
- views/css/style.css
  - Added will-change: transform to to .mover

- view/js/main.js
  - Rebuilt changeSliderLabel and changePizzaSizes per Cam's instructions in the Browser Rendering Optimization course
  - Updated updatePositions, putting lookups and calculations into variables and using those inside the for loop

- minified views/css/style.css using cssminifier.com
  - Saved as views/css/style-prod.css
- minified view/js/main.js using http://javascript-minifier.com
  - Saved as view/js/main-prod.js


References:
- Website Performance Optimization and Browser Rendering Optimization courses
- fend-office-hours/Web Optimization/Effective Optimizations for 60 FPS
- various suggestions offered on the Discussion Forum