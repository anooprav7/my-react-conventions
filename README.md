# Conventions

### Naming
* Functions in render functions which return a component needs to have its name start with render. Eg. A function which returns a block with a Clock, text and a Button will have the name renderClock or similar.
* When adding an event listener, the naming of the function should be 'on' and the event name follows as defined in the DOM functions. Eg. Callback for onClick function naming should start with onClick like onClickHandler or onClick itself. Callback for animationend should start with onAnimationEnd.

### Component functions
* When in class Components, inline class functions should be anonymous in nature. So the callback will only have a reference of the function. Eg. 
```
<Button onClick={this.onClick}>Click Me</Button>
```
