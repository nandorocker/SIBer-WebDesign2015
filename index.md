---
layout: default
---

{% for post in site.posts reversed %}
	{% capture current_module %}{{ post.module }}{% endcapture %}

	{% if current_module != module %}
## {% if post.module > 0 %}Module {{ current_module }} - {% endif %}{{ post.title }}
	{% capture module %}{{ current_module }}{% endcapture %}
	{% endif %}

- [{{ post.category | capitalize }}]({{ post.url | prepend: site.baseurl }})
{% endfor %}

# General Resources
- GOOGLE IS YOUR FRIEND
- Codecademy
- Lynda.com
- [w3schools](http://www.w3schools.com/cssref/default.asp)
- Nice code thread on [Quora](http://www.quora.com/I-want-to-learn-how-to-code-Im-about-to-turn-28-Is-it-too-late-to-learn-If-not-where-do-I-even-begin/answer/Ahmed-Balfaqih)
- [Bootstrap templates](http://startbootstrap.com)