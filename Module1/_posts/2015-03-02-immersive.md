---
layout: post
module: 1
title: "Intro to Style for the Web"
category: immersive
---

### View source, or why I <3 the open web
- Collaborative culture
- People create tools and share them, even competitors
- Small & large companies have the same shot
- Web always moving forward with community-created projects:
	- Frameworks (bootstrap, skeleton, foundation)
	- Preprocessors (LESS, SCSS, Jade)
	- Methodologies (SMACSS, BEM)


### But WTF is the internet?

	"It's a series of tubes"
	-- U.S. Sen. Ted Stevens, R-Alaska

#### 1960s

- ARPANET created based on academic work
- File transfer, communications
- Operated by military until its end, in 1990

#### 1990s

- 1989 - Tim Berners-lee [invents](http://www.w3.org/History/1989/proposal.html) the **Web + HTML** at *CERN*

![the www]({{ "/assets/Module1/" | prepend: site.baseurl }}wwwdiagram.jpg)

- 1993 - First Graphical Web Browser (Mosaic) made public
- 1995 - "Commercial internet" begins

*source: [six revisions](http://sixrevisions.com/resources/the-history-of-the-internet-in-a-nutshell/)*
	
### What is HTML?

- **H**yper**t**ext **M**arkup **L**anguage
- A way to **structure** content by using *tags*
	- Tags define the function of a block of text
	- Ex: header, paragraph, navigation, etc.
	- Tags are hierarchical: `html > body > p > etc`
- Interpreted by browsers

![Early HTML code]({{ "/assets/Module1/" | prepend: site.baseurl }}early_html.png)

Early HTML code [still around](http://sheldonbrown.com/web_sample1.html). It's rudimentary, yet still 100% readable.


### Content vs. Style

Early HTML mixed code & appearance:
{% highlight css %}

<font color="red" size="5">BIG FONT</font>
<table background="white" padding="2">...</table>
<blink>Everybody's favorite tag</blink>
	
{% endhighlight %}
- Creative design = lots of hacks
- Tables and spacer.gif
- Code is very busy, hard to read and edit

	
### Stylesheets
- Content file (html) separate from style file (css)
- **C**ascading **S**tyle **S**heets
- Cascading = children inherit parent attributes (less repetition)
- Box model allows great control of positioning

![Box Model]({{ "/assets/Module1/" | prepend: site.baseurl }}box_model.png)


### How it looks

![Basic CSS]({{ "/assets/Module1/" | prepend: site.baseurl }}syntax_nomenclature-diagram.png)

- Selectors
- Statements
	- Rules
	- Rule sets
	- At-rules
- Properties
- Comments


*Source: [CSS General class & nomenclature](http://reference.sitepoint.com/css/syntax)*

### How it works

- HTML tags
- Classes
	- Flexible: name it anything you like
	- Modular: can be applied to any HTML element
	- Many classes can be attached to the same element

- ID
	- Specific
	- Unique (can't repeat)
	- Should only be used for elements that may be manipulated

### Responsive design

- The mobile web and responsive design
- Technology changes how we consume content