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

![the www]({{ site.url }}assets/Module01/wwwdiagram.jpg)

- 1993 - First Graphical Web Browser (Mosaic) made public
- 1995 - "Commercial internet" begins

*source: [six revisions](http://sixrevisions.com/resources/the-history-of-the-internet-in-a-nutshell/)*
	
### What is HTML?

- **H**yper**t**ext **M**arkup **L**anguage
- A way to **structure** content by using *tags*
	- Tags define the function of a block of text
	- Ex: header, paragraph, navigation, etc.
	- Tags are hierarchical: `html > body > p > etc`

![Early HTML code]({{ site.url }}assets/Module01/early_html.png)

Early HTML code [still around](http://sheldonbrown.com/web_sample1.html). It's rudimentary, yet still 100% readable.


### Content vs. Style

Early HTML mixed code & appearance:

	<font color="red" size="5">BIG FONT</font>
	<table background="white" padding="2">...</table>
	<blink>Everybody's favorite tag</blink>
	
- Creative design = lots of hacks
- Tables and spacer.gif
- Code is very busy, hard to read and edit

	
### Stylesheets
- Content file (html) separate from style file (css)
- **C**ascading **S**tyle **S**heets
- Cascading = children inherit parent attributes (less repetition)
- Box model allows great control of positioning

![Box Model]({{ site.url }}assets/Module01/box_model.png)


#### What it looks like

![Basic CSS]({{ site.url }}assets/Module01/syntax_nomenclature-diagram.png)

- Selectors, statements (rules, rule sets and at-rules) and properties (Check out [CSS General class & nomenclature](http://reference.sitepoint.com/css/syntax))

Cascading: what are overrides?
- IDs vs. classes

- Scripting
	- Supports HTML/CSS
	- Extends page functionality & behavior
	- Shouldn't be used in place of good, valid HTML/CSS

### Responsive design

- Ask: who knows what it means?
- The mobile web and responsive design
- How small screens change


## Debrief

- Q&A's
- Ask students to email me when lab assignments are done