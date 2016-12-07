#HSLIDE
## JavaScript

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

###scripting language

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
## strict mode
* `use strict` at the beginning of a script or function 

An optional mode to write code in a more restricted JavaScript variant, as for example:
* do not allow using undeclared variables
* do not allow object properties with the same name
* do not allow deleting variables or functions
* do not allow escape characters
* ...

#HSLIDE
## Declarations
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
* command line, via custom modules (e.g. `prompt`in node.js)
* requests
* ...

#HSLIDE
## Objects 
```javascript
// object literal declaration
var person = {
firstname: 'James',
say: function () { console.log('hi'); }
};

// properties and method access
console.log(person.name);
person.say('hi');

// reassign values
person.say = function (something) {console.log(something)};

// add new properties
person.lastname = "Waits";
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
person.talk('hi');

// reassign values
person.talk = function (something) {console.log(something)};

// add new properties
person.age = 33;
```

#HSLIDE
## Object properties access 

```javascript
// object properties can be anything
// including (nested) objects
person.name = {
  first : "Chivas",
  last : "Regal"
}

// arrays (of any kind of values)
person.programming = ['JavaScript','C/C++'];
```

