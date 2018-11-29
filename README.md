# Conventions

## 1 Naming
#### 1.1 Rules common to all identifiers
Identifiers use only ASCII letters and digits, and, in a small number of cases noted below, underscores and very rarely (when required by frameworks like Angular) dollar signs.
Give as descriptive a name as possible, within reason. Do not worry about saving horizontal space as it is far more important to make your code immediately understandable by a new reader. Do not use abbreviations that are ambiguous or unfamiliar to readers outside your project, and do not abbreviate by deleting letters within a word.
```
priceCountReader      // No abbreviation.
numErrors             // "num" is a widespread convention.
numDnsConnections     // Most people know what "DNS" stands for.
```
Illegal
```
n                     // Meaningless.
nErr                  // Ambiguous abbreviation.
nCompConns            // Ambiguous abbreviation.
wgcConnections        // Only your group knows what this stands for.
pcReader              // Lots of things can be abbreviated "pc".
cstmrId               // Deletes internal letters.
kSecondsPerDay        // Do not use Hungarian notation.
```
#### 1.2 Rules common to all identifiers 

### React Specific
* Functions in render functions which return a component needs to have its name start with render. Eg. A function which returns a block with a Clock, text and a Button will have the name renderClock or similar.
* When adding an event listener, the naming of the function should be 'on' and the event name follows as defined in the DOM functions. Eg. Callback for onClick function naming should start with onClick like onClickHandler or onClick itself. Callback for animationend should start with onAnimationEnd.

### Component functions
* When in class Components, inline class functions should be anonymous in nature. So the callback will only have a reference of the function. Eg. 
```
<Button onClick={this.onClick}>Click Me</Button>
```
