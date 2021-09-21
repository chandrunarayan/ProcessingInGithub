# Java Program runs in Processing but not on GitHub
Some common problems that could cause your program not to work on the web are:
- Using `circle()`, `square()`,`clear()`, `delay()`, `push()`, `pop()` or other functions that aren't implemented in [processing.js](http://processingjs.org/reference/)
- Leaving the debugging tools `System.out.println()` or `System.out.print()` in your finished program
- Naming a variable with the same name as a function
- Naming two variables with the same name
- Naming a function or a variable with a name that is already used in Processing
- Using `CHORD` or `PIE` modes with `arc()`
- Using an image as an argument in `background()`
- Using decimals for x and y coordinates
- Integer division
- Extra curly braces and/or semi-colons
- No spaces in an `ArrayList` declaration or initialization (e.g. `ArrayList<Integer>someList` instead of `ArrayList <Integer> someList`)
- Calling the `ArrayList` function `removeAll()`
- The name of the `.pde` file doesn't match the name in the canvas id tag in `index.html`
- If you are using multiple `.pde` files you will need to list them in `index.html` using a canvas tag like `<canvas id="AsteroidsGame" data-processing-sources="Asteroid.pde AsteroidsGame.pde Floater.pde Spaceship.pde Star.pde"> </canvas>`

To display our AP Java programs on the web, we're using [processing.js](http://processingjs.org/). Not all Processing functions are compatible with processing.js. You can check [this list](http://processingjs.org/reference/) to see if you are using a function that isn't supported. 

Looking for error messages can also provide clues to the problem. You can find the error messages for your webpage by opening the *web console* or *javascript console* in your browser. To open the console in Chrome, press the F12 key. To open the console in Firefox, use Ctrl + Shift + J.
