#HSLIDE
# JavaScript Intro

#HSLIDE
## History
* 1995: At Netscape, Brendan Eich created LiveScript (then renamed to "JavaScript")
* 1996: Microsoft releases "JScript", a port for IE3.
* 1997: JavaScript was standardized in the "ECMAScript" spec.
* 2005: "AJAX" was coined and the web 2.0 age begins.
* 2006: jQuery 1.0 was released.
* 2010: Node.JS was released.
* 2015: ECMAScript 6 was released (lots of new features)
* 2016: ECMAScript 7 was released (small release)

#HSLIDE
## What it is
### JavaScript is a
* cross-platform
* object-oriented
* dynamically typed
* small and lightweight

### scripting language

#HSLIDE
## Where it is used
### web @client side (browser)
* document manipulation (DOM scripting)
* interfacing with Web APIs 
* asynchronous requests
* interaction & animation
* ...

#HSLIDE
## Where it is used
### web @server side
* server runtime environment (node.js)
* databases (MongoDB, CouchDB)
* workflow automation (e.g. Gulp)
* transpilers (Coffee Script, Babel)
* ...

#HSLIDE
## Where it is used
### @many other applications
* game engines (Unity 3D)
* document producers (Adobe Acrobat)
* GUI (GNOME)
* embedded computers and micro-controllers (Espruino)
* ...

#HSLIDE
## Syntax & Grammar
* case sensitive
* statements (instructions) separeted by ";"
* inline comments 
 * `// comment until end of line`
* block comments 
 * `/* comment until closed */`


#HSLIDE
## Data Types
* Number (IEEE double float)
* String
* Boolean
* Object (Function, Array, Date, RegExp)

* `undefined` and `null` (special)
* Symbol (immutable, new in ES6)

#HSLIDE
## Literals
1. Numbers:`1, 2, 3, 1.28e4, NaN, Infinity`
2. Strings: `'xyz', 'foo \n', '\u2603'`
3. Boolean: `true, false`
4. Objects: `{post: 'hello world', title: 'hello', userid : 123}`
5. Array: `[1, 2, 'queijo', 'beijo']`
6. Functions:
```javascript
var cube = function (x) {
      return x * x * x;
}
```

#HSLIDE
##Strings
* Strings may be enclosed with single quotes or double quotes.  
* Escape characters use backslash `'\n \t \\'`
* Strings are *immutable* - once created, you can't change them (e.g. concatenating with the `+` operator returns a new string)
* There is no `char` - just use strings of length 1
* Many methods/properties &ndash; `.length, substring(), toLowerCase(), toUpperCase()` ...
* documentation [MDN string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)


#HSLIDE
##Arrays
* Literal notation uses square brackets: `['foo', 'bar', baz']`
* Can be heterogenous: `['foo', 1, true]`
* Elements accessed with square bracket notation: `arr[0]`
* several methods like `push(), pop(), slice(), shift(), unshift()`
* documentation: [MDN Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)


#HSLIDE
##Booleans

* `true` and `false`
* Standard logical operators (`&&, ||, !`)
* JavaScript isn't statically typed : ANY value can be used with a logical operator
  * *Falsy* values: `false, null, undefined, 0, NaN, ''`
  * Any other value is *truthy* (including `'false', [], {}`)


#HSLIDE
## Operators

* numeric: +, -, *, /
* numeric: % (remainder)
* inc & dec : ++ , -- (prefix or postfix)
* assignment: =
* coumpound: =*, =-, ...
* string concatenation: +

#HSLIDE
## Operators
* comparison: <, >, =>, <=
* comparison with type coercion : ==, !==
* comparison without type coercion : ===, !===
* boolean : && (and), || (or), ! (not)
* ternary: cond1 ? exp_if_true : else

#HSLIDE
## Control Structures
* if () {}
* if () else {}
* if () elseif {} elseif {} else {}

#HSLIDE
## Control Structures
* do {} while ()
* while () {}
* for (;;) {}
* for (let value of array) {} // arrays
* for (let prop in object) {} // objects
* switch () {case v1: s1; break; ... default : sd; }


#HSLIDE
## strict mode
* `use strict` at the beginning of a script or function 

An optional mode to write code in a more restricted JavaScript variant, as for example:

* do not allow using undeclared variables
* do not allow object properties with the same name
* do not allow deleting variables or functions
* do not allow escape characters
* ...

#HSLIDE
## Scope
* `let`
 * Declares a block scope local variable, optionally initializing it to a value.
* `var`
 * Declares a variable, optionally initializing it to a value.
* `const`
 * Declares a read-only named constant.

#HSLIDE
## Output
JavaScript has no built-in input / output.

but it can display to ...

* to the console (browser, node.js, other environments)
* to window alert boxes (browsers)
* to HTML documents (via write ou innerHTML)
* ...


#HSLIDE
## Input
JavaScript has no built-in input / output.

but it can read data from ...

* prompt windows (browsers)
* HTML forms (HTML document)
* command line, via custom widgets (e.g. `prompt`in node.js)
* requests
* ...

#HSLIDE
##Functions

* First-class object (this allows JS to take advantage of functional programming techniques)
* Functions can return a value with the `return` keyword
* If no value is returned, then the function returns `undefined`

```javascript
var cube = function (x) {
  return x * x * x;
}
```

#HSLIDE
##Functions vs Calls

A function call is very different from the function itself! A function call ends with parentheses.

```javascript
var cube = function (x) {
  return x * x * x;
}

console.log(cube); // logs the function object
console.log(cube(2)); // logs the result of the function call
```



#HSLIDE
## Functions 

```javascript
function add(x, y) {
  var total = x + y;
  return total;
}
add(); // NaN
add(2, 3, 4); // 5
```

#HSLIDE
## Function arguments

```javascript
function add() {
  var sum = 0;
  for (var i = 0, j = arguments.length; i < j; i++) {
    sum += arguments[i];
  }
  return sum;
}
add(2, 3, 4, 5); // 14
```
#HSLIDE
## Function arguments


```javascript
function avg(...args) {
  var sum = 0;
  for (let value of args) {
    sum += value;
  }
  return sum / args.length;
}

avg(2, 3, 4, 5); // 3.5
```
#HSLIDE
## Anonymous functions
```js
var avg = function() {
  var sum = 0;
  for (var i = 0, j = arguments.length; i < j; i++) {
    sum += arguments[i];
  }
  return sum / arguments.length;
};

avg(1,2,3,4,5); // 3.4

```
#HSLIDE
## Creating context with IIFE
#### immediate invoked function expression
```js
var a = 1;
var b = 2;

(function() {
  var b = 3;
  a += b;
})();

a; // 4
b; // 2
```


#HSLIDE
## recursive functions
```js
function fibonacci(num) {
  if (num <= 1) return 1;

  return fibonacci(num - 1) + fibonacci(num - 2);
}
```


#HSLIDE
## Objects

* Lightweight, mutable key-value stores
* Literal notation uses curly braces: `{foo: 'bar', 'baz': 2}`
* Property names can be strings: `{'foo': 'bar'}`
* Access with `obj.propertyName` **or** `obj['propertyName']`

#HSLIDE
## Everything is an Object

* Aside from the primitive types (String, boolean, and Number) - everything in JS is a kind of object
  - Even primitives can behave like objects (Strings, for example, have properties/methods)
* Array is an object with integer keys and specific methods (e.g. `splice(), indexOf()`)
* Functions are also object-like, and can have properties and methods. Can be thought of as *executable objects*


#HSLIDE
## Objects
```javascript
var obj = {
    someProperty: 'abcdef',
    nestedObject: { a: 1, b: 2, c: 3 },
    func: function () { 
      return 0;
    }
  }

  obj.someProperty        // --> 'abcdef'
  obj['nestedObject'].a   // --> 1
```


#HSLIDE
## Objects
```javascript
// object literal declaration
var person = {
name: 'James',
talk: function () { console.log('hi'); }
};

// properties and method access
console.log(person.name);
person.talk();

// reassign values
person.talk = function (something) {console.log(something)};

// add new properties
person.age = 33;
```

#HSLIDE
## Object properties 

```javascript
// object properties can be anything
// including (nested) objects
person.name = {
  first : "Chivas",
  last : "Regal"
}

person.talk("my name is " + 
					person.name.first + " " +
					person['name']['last']);
					
// arrays (of any kind of values)
person.programming = ['JavaScript','C/C++'];
```

#HSLIDE
## Object property this

```javascript
var person2 = {
name: 'James',
talk: function () { console.log('I am ' + this.name); }
};

person2.talk();
```
#HSLIDE
## Function property this
* When a function is not assigne to an object, the `this` represents the **Global object**.
 * in web browsers `this` is the Window object.
 * in node `this` is a `global` object.

```javascript
var talk =  function () { console.log('I am ' + this); };
talk();
```
