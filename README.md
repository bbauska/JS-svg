# JS-SVG
## JavaScript and SVG Generative Art with JavaScript and SVG
### Utilizing Scalable Vector Graphics and Algorithms for Creative Coding and Design

Design Thinking is a set of strategic and creative processes and principles
used in the planning and creation of products and solutions to human-
centered design problems.
With design and innovation being two key driving principles, this
series focuses on, but is not limited to, the following areas and topics:

  - User Interface (UI) and User Experience (UX) Design
  - Psychology of Design
  - Human-Computer Interaction (HCI)
  - Ergonomic Design
  - Product Development and Management
  - Virtual and Mixed Reality (VR/XR)
  - User-Centered Built Environments and Smart Homes
  - Accessibility, Sustainability and Environmental Design
  - Learning and Instructional Design
  - Strategy and best practices

This series publishes books aimed at designers, developers, storytellers
and problem-solvers in industry to help them understand current
developments and best practices at the cutting edge of creativity, to invent
new paradigms and solutions, and challenge Creatives to push boundaries
to design bigger and better than before.

# Generative Art with JavaScript and SVG Utilizing Scalable Vector Graphics and Algorithms for Creative Coding and Design

## Introduction
### What You Should Know
As a reader, what should you know before tackling this book? It will
no doubt be easier if you are comfortable with the core concepts of
programming, like variables, functions, loops, and conditionals. These
kinds of concepts carry over from language to language, differing mainly
with respect to syntax, so if you come from a language other than
JavaScript, then that’s completely fine.
If you have no prior programming experience, we will be covering
the concepts required in Chapter 2, but I should emphasize that this
book is not intended to be an introduction to programming. The second
chapter is best thought of as a primer, a jumping-off point for a deeper
dive elsewhere. A short introductory course would really benefit you here.
Personally I’d recommend the wonderful freeCodeCamp.com, a site I’ve
spent many hours using myself. It offers free interactive tutorials on the
basics of HTML, CSS, and JavaScript, and much more besides.
For those coming from another language, like Python, PHP, or C#, the
second chapter may still be valuable, to be sure you’re acquainted with the
syntax and some of the idiosyncrasies of JavaScript.
If you’re already a practicing web developer, you could skip (or
quickly skim) Chapter 2, depending on your level of experience. If you’re
unfamiliar with any of the techniques or syntax used in our opening
example (which we’ll end Chapter 1 with), I’d encourage you to give the
second chapter a read, where they’ll be fully explained. The field of web
development is vast enough that what is bread and butter to one developer
might be bleeding edge to another.

### Tools
On the tool end of things, we’ll be using the following:
  - JavaScript and the SvJs library. I’ll elaborate on this further later.
  - A code editor. Here I’ll be giving you a choice between
    - Visual Studio Code (an excellent open source code editor)
    - CodePen (a popular online code editor)
  - If you opt to use Visual Studio Code (which I recommend), we’ll also be using Node.js and NPM to manage dependencies (a good habit to get into as a developer).

All code examples are available on both GitHub and CodePen, so feel
free to follow along whichever way you prefer. You can of course do both,
work locally with a code editor but check out CodePen examples online for
quick inspiration. For convenience, I’ll organize and embed all CodePen
examples at davidmatthew.ie/generative-art-javascript-svg.

### Techniques
In terms of the techniques we’ll tackle, by the end of this book, you should
have a good overview of the following:
  - The main functionality of the SvJs library and how it relates to the SVG spec
  - Creating generative art sketches with JavaScript using ES6+ syntax
  - Generating primitive SVG shapes
  - Creating iterative variations of sketches by randomizing parameters
  - Using noise to create organic variance
  - Generating complex SVG paths
  - Making sketches interactive
  - Animating sketches
  - Using SVG filters generatively

We’ll be covering a lot of ground, so don’t put yourself under pressure
to understand everything. I must have encountered certain programming
concepts umpteen times before the proverbial penny finally dropped
(JavaScript promises anyone?), and whenever understanding did finally
dawn, it would usually be because I was experimenting with something I
wanted to build, rather than repeating tutorial steps by rote. Tutorials and
instructional books certainly have their place (I wouldn’t be writing this
book otherwise), but it’s important that you take what you want from them,
rather than seeing them as syllabi to be strictly followed.
A sense of play is important, particularly when it comes to art. And
although I mentioned tools previously, I would prefer if you viewed this
book as more of a toybox than a toolbox. When I think of tools, I think of
problems that need fixing, like the loose hinges on that crooked cabinet
you’re going to tighten any day now. Tools tend to be more functional than
fun, and I’d like you to have some fun with this book.

## The Beginner’s Path
Before journeying along any path, the groundwork needs to be in place.
In this opening chapter, that’s what we’ll do, lay the groundwork. We’ll
introduce SVG, explain what makes it a uniquely powerful image format,
and show how it can be used with JavaScript to create generative art. In the
process, we’ll set up our tools and a template we can use for subsequent
sketches.
### Why JavaScript and SvJs?
Most books about generative art use a Java-based language called
Processing, or its JavaScript port p5.js. Processing was created specifically
for artists and designers new to coding and has a large and active
community. So why doesn’t this book use it?
My first forays into generative art were with Processing, so I certainly
acknowledge its value. I quickly moved to p5.js when the library was first
released in 2013, which allowed generative sketches to be written directly
in JavaScript, the language of the Web. But when I wanted to integrate
some of my own sketches into real-world web development projects, its
limitations quickly showed. It’s a large library, clocking in at close to a
megabyte at last check, and while that may not sound like much, it’s a lot
by web development standards.

