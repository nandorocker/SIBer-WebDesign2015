---
module: 5
title: "Intro to jQuery & JS Libraries"
category: immersive
layout: default
---

# Java-what?

## On a scale of 1-5, how much programming have you done? Which languages?

## The triad:

- **HTML**: content
- **CSS**: style
- **Javascfipt**: behavior

## What's Javascript for?

- On client-side, mostly used for **behavior** on pages
- Also used on the server-side (NodeJS)


## Some examples

- Show some websites with JS functionality

## Let's creat a program.

1) Create a simple HTML page:

```html
<html>
	<head>
		<title>Testing Javascript</title>
	</head>
	<body>
		
	</body>
</html>

```

2) Add the `script` tag just before closing the `body`:

```html
<html>
	<head>
		<title>Testing Javascript</title>
	</head>
	<body>
		
		<script>
			
		</script>
	</body>
</html>

```

3) Within the `script` tag, add the command:

```javascript
alert("Hello world");
```

4) Open the browser and you should see this:

![Alert](http://shots.nan.do/image/3h1m1Z3j3Z2K/Image%202015-03-22%20at%2012.14.52%20AM.png)

## Your program has two parts:

### alert( )

Function

### "Hello world"

String

## Inline scripting is not recommended. Let's link to an external document:


```html

		...
		<script src="js/your_filename.js"></script>
	</body>

```

## Testing Javascript

### Chrome Inspector Console
![Chrome](http://shots.nan.do/image/1w3T252F2x37/Image%202015-03-22%20at%2012.32.05%20AM.png)

### Firefox Inspector Console
![Firefox](http://shots.nan.do/image/2b2j1a1n0Z02/Image%202015-03-22%20at%2012.29.29%20AM.png)

### Node REPL
![Node](http://shots.nan.do/image/023x250V0F3L/Image%202015-03-22%20at%2012.27.24%20AM.png)

## Let's refactor

```javascript

var sayIt = function(message) {
	alert(message);
}

var myMessage = "Hello Berlin!";

sayIt(myMessage);

```

## Breaking it down

```javascript

// Function declaration
var sayIt = function(message) {
	alert(message);
}

// Variable assignment
var myMessage = "Hello Berlin!";

// Function invocation
sayIt(myMessage);

```

# Stuff you'll get with Javascript:
## Logic

```javascript

if (message === 'Hello Berlin!') {
	alert(message);
} else {
	alert('Something else was set.');
}

```

```javascript

if (typeof window != 'undefined') {
	alert(message);
} else {
	console.log(msg);
}

```

## Regular expressions
## Loops and iteration
## Arrays
## Objects

# jQuery: what is it?

- A popular Javascript framework
- Created by John Resig
- Simplifies cross-browser behavior for animation, event handling, **AJAX** and **DOM** manipulation

# Why is it so popular?

- Lightweight
- Easy to learn using familiar CSS syntax and intuitive 
- Many plugins available 
- Easy to extend and compatible 
- Rich community
- Readable: can you read this?

```javascript
$('#something').hide().css('background', 'red').fadeIn();
```

# What is DOM?

## Document Object Model

**Cross-platform** and **language-independent** convention to represent and interact with **objects** in HTML, XHTML and XML documents

![DOM](http://shots.nan.do/image/1M3m0p40223s/DOM.png)

# Diving into jQuery

## First step: load up jQuery (CDN)

```html

<head>
...
<script src="//code.jquery.com/jquery-2.1.3.min.js"></script>
...
</head>

```

## The jQuery function:

```javascript

$(<selector>);

$(function(){}); // alias for $(document).ready

$(<html><markup>);

```

## Selectors

Consider this bit of HTML:

```html

<a href="hello.html"
   class="greeting"
   style="color: blue;"
   id="greeter">Say hello</a>

```

There are many ways we can identify this specific element:

```javascript

$("a");

$("a:first");

$("a.greeting")

$("#greeter") // Most efficient selector

```

---

# What Can I Do With a Selector?

```javascript

$("a").css("color"); //the color of a: blue

$("a").offset().top; //position of the element

$("a").hide(); //hide the element

$("a").remove(); //remove the element

$("a").addClass("context"); //add a class

$("a").after("<p>Hello</p>")); //append

```

# What Can I Do With a Selector?

```javascript

$("a").css("color"); DOM

$("a").offset().top;

$("a").hide(); Manipulation

$("a").remove();$("a").addClass("context");

$("a").insertAfter($("<p>Hello</p>"));

```

# Let's look at some examples

- Events
- Reacting to input

---

# Sources

This presentation was strongly based off of Dan Pickett's [Introduction to Javascript and jQuery](http://www.slideshare.net/enlightsolutions/intro-to-jquery-16383771) and Gill Clereen's [Getting started with jQuery](http://www.slideshare.net/gillcleeren/getting-started-with-jquery-33853415).