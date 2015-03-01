---
layout: default
---

# {{ site.title }}

### by nando rossi

{% for post in site.posts reversed %}
- [{{ post.title }}]({{ post.url | prepend: site.baseurl }})
{% endfor %}

# General Resources
- GOOGLE IS YOUR FRIEND
- Codecademy
- Lynda.com
- [w3schools](http://www.w3schools.com/cssref/default.asp)
- Nice code thread on [Quora](http://www.quora.com/I-want-to-learn-how-to-code-Im-about-to-turn-28-Is-it-too-late-to-learn-If-not-where-do-I-even-begin/answer/Ahmed-Balfaqih)
- [Bootstrap templates](http://startbootstrap.com)