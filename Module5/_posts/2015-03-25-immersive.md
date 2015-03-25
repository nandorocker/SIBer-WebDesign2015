---
module: 5
title: "Intro to jQuery & JS Libraries"
category: immersive
layout: default
---

# jQuery

## The usual triad:

- **HTML**: content
- **CSS**: style
- **Javascfipt**: behavior
	
# Javascript for behavior

Here's some sites that use JS:

- [Galleries](http://gallagalla.com)
- Animated navigations like [this](https://www.140c.com)
- Automatic feeds (Twitter, Gmail)
	
# Javascript changes your page dynamically

- When a user does something
- When content is updated on a server
- At a certain day of the year
- etc.

# jQuery makes Javascript accessible

jQuery is a Javascript framework. It enables a non-developer to do complicated things.

- Usind jQuery without knowing Javascript = doing Bootstrap without CSS
- jQuery looks closer to CSS
	

# Let's watch a [video](http://try.jquery.com/levels/1/sections/2)!

# DOM: The Document Object Model

- How **browsers** identify the content on a website
- Also the order things load
- Divided in **nodes**
- Set up like a tree (DOM tree):
	- Parents
	- Children
	- Siblings

# Demos from [jQuery](http://try.jquery.com/levels/1/sections/3)

## Simple Element Selector

## Document Ready
```javascript

$(document).ready(function() {

});

```

## Descendant selectors/immediate child

## Using jQuery's traversal for speed


```css
#travel .offer { }

```

```javascript

$("#travel").find(".offer");

```

```css
#travel > li { }

```

```javascript

$("#travel").child("li");

```

```css
#travel > li:first { }

```

```javascript

$("#travel").child("li").first();

```

### Download presentation

Presentation [here]({{ "/assets/Module4/" | prepend: site.baseurl }}module5-immersive.pdf)