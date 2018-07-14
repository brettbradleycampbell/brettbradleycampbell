---
layout: page
title: clients
permalink: /clients
---

<div>
{% for page in site.pages %}
	<ul>
	{% if page.category == 'clients' %}	
		<li><a href="{{ page.url }}">{{ page.title }}</a></li>
	{% endif %}
	</ul>
{% endfor %}
</div>