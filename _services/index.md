---
layout: page
title: services
permalink: /services
---

<ul>
	{% for page in site.services %}
	{% if page.path contains 'index' %}
	{% else %}
	<li><a href="{{ page.url }}"><span>{{ page.title }}</span></a></li>
	{% endif %}
	{% endfor %}
</ul>