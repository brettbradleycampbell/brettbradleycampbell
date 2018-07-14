---
layout: page
title: services
permalink: /services
---

<div>
{% for page in site.pages %}
	<ul>
	{% if page.category == 'services' %}	
		<li><a href="{{ page.url }}">{{ page.title }}</a></li>
	{% endif %}
	</ul>
{% endfor %}
</div>