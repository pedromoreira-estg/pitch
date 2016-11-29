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
## Output
JavaScript has no built-in input / output.

but it can read data from ...
* prompt windows (browsers)
* HTML forms (HTML document)
* command line, via custom modules (e.g. `prompt`in node.js)
* requests
* ...

#HSLIDE
## Object Literals 

```javascript
var person = {
name: "James",
say: function (something) { console.log(something); }
};
```



#HSLIDE

## The Kitchen Sink
##### <span style="font-family:Helvetica Neue; font-weight:bold">A <span style="color:#e49436">Git</span>Pitch Feature Tour</span>

#HSLIDE
## Slideshow Theme Switcher
<span style="font-size:0.6em; color:gray">Available bottom-left of screen.</span> |
<span style="font-size:0.6em; color:gray">Start switching themes right now!</span>

#HSLIDE

## Tip!
For best viewing experience press **F** key to go fullscreen.

#HSLIDE

## Markdown Slides
<span style="font-size:0.6em; color:gray">Press Down key for details.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Slide-Markdown" target="_blank">GitPitch Wiki</a> for details.</span>


#VSLIDE

#### Use GitHub Flavored Markdown
#### For Slide Content Creation

<br>

The same tool you use to create project **READMEs** and **Wikis** for your Git repos.

#HSLIDE

## Code Slides
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Code-Slides" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Use Markdown Code Blocks

<br>

And enjoy code syntax highlighting for dozens of languages powered by <a target="_blank" href="highlight.js](https://highlightjs.org">highlight.js</a>.

#VSLIDE

```JavaScript
// JavaScript Code Block

$('button').click(function(){
    $('h1, h2, p').addClass('blue')
    $('div').removeClass('important')
    $('h3').toggleClass('error')
    $('#foo').attr('alt', 'Lorem Ipsum')
});
```

#VSLIDE

```Scala
// Scala Code Block

HashMap params = HashMap(n -> 10, mean -> 5)

// Define executable for R stats#rnorm function call.
OCPUTask task = OCPU.R()
                    .pkg("stats")
                    .function("rnorm")
                    .input(params.asJava)
                    .library()
```

#VSLIDE

```Go
// Go Code Block

package main

import "fmt"

func swap(x, y string) (string, string) {
    return y, x
}

func main() {
    a, b := swap("hello", "world")
    fmt.Println(a, b)
}
```

#HSLIDE

## GIST Slides
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/GIST-Slides" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### GitHub GIST
#### Building Blocks For Any Presentation

<br>

Enjoy 100% reusable code snippets, excellent syntax highlighting, code indentation and styling. 

#VSLIDE?gist=8da53731fd54bab9d5c6

#VSLIDE?gist=28ee3d19ddef9d51b15adbdfe9ed48da

#HSLIDE

## Image Slides
## [ Inline ]
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Image-Slides" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Make A Visual Statement

<br>

Use inline images to lend a *visual punch* to your slideshow presentations.


#VSLIDE

<span style="color:gray; font-size:0.7em">Inline Image at <b>Absolute URL</b></span>

![Image-Absolute](https://d1z75bzl1vljy2.cloudfront.net/kitchen-sink/octocat-privateinvestocat.jpg)

<span style="color:gray; font-size: 0.5em;">the <b>Private Investocat</b> by <a href="https://github.com/jeejkang" target="_blank">jeejkang</a></span>


#VSLIDE

<span style="color:gray; font-size:0.7em">Inline Image at GitHub Repo <b>Relative URL</b></span>

![Image-Absolute](assets/octocat-de-los-muertos.jpg)

<span style="color:gray; font-size:0.5em">the <b>Octocat-De-Los-Muertos</b> by <a href="https://github.com/cameronmcefee" target="_blank">cameronmcefee</a></span>


#VSLIDE

<span style="color:gray; font-size:0.7em"><b>Animated GIFs</b> Work Too!</span>

![Image-Relative](https://d1z75bzl1vljy2.cloudfront.net/kitchen-sink/octocat-daftpunkocat.gif)

<span style="color:gray; font-size:0.5em">the <b>Daftpunktocat-Guy</b> by <a href="https://github.com/jeejkang" target="_blank">jeejkang</a></span>

#HSLIDE

## Image Slides
## [ Background ]
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Image-Slides#background" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Make A Bold Visual Statement

<br>

Use high-resolution background images for maximum impact.

#VSLIDE?image=https://d1z75bzl1vljy2.cloudfront.net/kitchen-sink/victory.jpg

#VSLIDE?image=https://d1z75bzl1vljy2.cloudfront.net/kitchen-sink/127.jpg


#HSLIDE

## Video Slides
## [ Inline ]
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Video-Slides" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Bring Your Presentations Alive

<br>

Embed *YouTube*, *Vimeo*, *MP4* and *WebM* inline on any slide.

#VSLIDE

![YouTube Video](https://www.youtube.com/embed/dNJdJIwCF_Y)

#VSLIDE

![Vimeo Video](https://player.vimeo.com/video/125471012)

#VSLIDE

![MP4 Video](http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4)


#HSLIDE

## Video Slides
## [ Background ]
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Video-Slides#background" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Maximize The Viewer Experience

<br>

Go fullscreen with *MP4* and *WebM* videos.

#VSLIDE?video=http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4

#HSLIDE

## Math Notation Slides
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Math-Notation-Slides" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE


#### Beautiful Math Rendered Beautifully

<br>

Use *TeX*, *LaTeX* and *MathML* markup powered by <a target="_blank" href="https://www.mathjax.org/">MathJax</a>.

#VSLIDE

`$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$`

#VSLIDE

`\begin{align}
\dot{x} & = \sigma(y-x) \\
\dot{y} & = \rho x - y - xz \\
\dot{z} & = -\beta z + xy
\end{align}`

#VSLIDE

##### The Cauchy-Schwarz Inequality

`\[
\left( \sum_{k=1}^n a_k b_k \right)^{\!\!2} \leq
 \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
\]`

#VSLIDE

##### The probability of getting \(k\) heads when flipping \(n\) coins is:

`\[P(E) = {n \choose k} p^k (1-p)^{ n-k} \]`

#VSLIDE

##### In-line Mathematics

This expression `\(\sqrt{3x-1}+(1+x)^2\)` is an example of an inline equation.

#HSLIDE

## Slide Fragments
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Fragment-Slides" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Reveal Slide Concepts Piecemeal

<br>

Step through slide content in sequence to slowly reveal the bigger picture.

#VSLIDE

- Java
- Groovy     <!-- .element: class="fragment" -->
- Kotlin     <!-- .element: class="fragment" -->
- Scala     <!-- .element: class="fragment" -->
- The JVM rocks! <!-- .element: class="fragment" -->

#VSLIDE

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th> 
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>25</td>
  </tr>
  <tr class="fragment">
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
  <tr class="fragment">
    <td>John</td>
    <td>Doe</td>
    <td>43</td>
  </tr>
</table>

#HSLIDE
## <span style="text-transform: none">PITCHME.yaml</span> Settings
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Slideshow-Settings" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Stamp Your Own Look and Feel

<br>

Set a default theme, custom logo, custom css, background image, and preferred code syntax highlighting style.

#VSLIDE

#### Customize Slideshow Behavior

<br>

Enable auto-slide with custom slide intervals, presentation looping, and RTL flow.


#HSLIDE
## Slideshow Keyboard Controls
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Slideshow-Fullscreen-Mode" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Try Out These Great Features Now!

<br>

| Mode | On Key | Off Key |
| ---- | :------: | :--------: |
| Fullscreen | F |  Esc |
| Overview | O |  O |
| Blackout | B |  B |
| Help | ? |  Esc |


#HSLIDE

## GitPitch Social
<span style="font-size:0.6em; color:gray">Press Down key for examples.</span> |
<span style="font-size:0.6em; color:gray">See <a href="https://github.com/gitpitch/gitpitch/wiki/Slideshow-GitHub-Badge" target="_blank">GitPitch Wiki</a> for details.</span>

#VSLIDE

#### Slideshows Designed For Sharing

<br>

- View any slideshow at its public URL
- [Promote](https://github.com/gitpitch/gitpitch/wiki/Slideshow-GitHub-Badge) any slideshow using a GitHub badge
- [Embed](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Embedding) any slideshow within a blog or website
- [Share](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Sharing) any slideshow on Twitter, LinkedIn, etc
- [Print](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Printing) any slideshow as a PDF document
- [Download and present](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Offline) any slideshow offline

#HSLIDE

## GO FOR IT.
## JUST ADD <span style="color:#e49436; text-transform: none">PITCHME.md</span> ;)
