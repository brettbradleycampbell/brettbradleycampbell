---
layout: default
title: clients
permalink: /clients
order: 0
---

<div class="grid client-images">
	{% for page in site.clients %}
	{% if page.path contains 'index' %}
	{% else %}
	<div class="grid__item medium-up--one-half">
		<li><a href="{{ page.url }}"><span><img src="{{page.image}}"></span></a></li>
	</div>
	{% endif %}
	{% endfor %}
</div>
