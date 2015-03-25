### Module 5
# Introduction to jQuery
## "Write less, do more"

---

## The usual triad:

- **HTML**: content
- **CSS**: style (sometimes behavior)
- **Javascfipt**: behavior (sometimes style)

![eye](http://img1.wikia.nocookie.net/__cb20121208115833/deusex/en/images/8/8e/All_seeing_eye.jpg)

	
---

# CSS for behavior

---

## CSS3 + HTML5 allow for lots of nice things:
- Transitions
- Animations
- Hover state

---

# Javascript for behavior

--- 

## Some live examples:

- [Galleries](http://gallagalla.com)
- Animated navigations like [this](https://www.140c.com)
- Automatic feeds (Twitter, Gmail)

---

## Javascript can:

- Respond to user interactions
- Handle live updates on a server
- Change the style/content of a page in real-time
- Create fancy effects

---

## Downsides

- Adds overhead to page
- Lots of stuff can be done with CSS3 + HTML5
- Some users/devices disable JS
- Screen readers may ignore it

---

# Javascript takes a lot of practice.

---

# ENTER: JQUERY.

---

## jQuery is a Javascript framework that enables front-end devs to do complicated things.

---	

# Let's watch a [video](http://try.jquery.com/levels/1/sections/2)!

---

# DOM: The Document Object Model

- How **browsers** identify the content on a website
- Also the order things load
- Divided in **nodes**
- Set up like a tree (DOM tree):
	- Parents
	- Children
	- Siblings

---

## Testing Javascript

---

### Chrome Inspector Console
![Chrome](http://shots.nan.do/image/1w3T252F2x37/Image%202015-03-22%20at%2012.32.05%20AM.png)

---

### Firefox Inspector Console
![Firefox](http://shots.nan.do/image/2b2j1a1n0Z02/Image%202015-03-22%20at%2012.29.29%20AM.png)

---

### Node REPL
![Node](http://shots.nan.do/image/023x250V0F3L/Image%202015-03-22%20at%2012.27.24%20AM.png)

---

# Do some demos from [jQuery](http://try.jquery.com/levels/1/sections/3)

---

## Simple Element Selector

---

## Document Ready
```javascript

$(document).ready(function() {

});

```

---

## Descendant selectors/immediate child

---

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