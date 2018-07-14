---
layout: page-client
title: Jen Kane
category: 'clients'
services:
- branding 
- graphic design
description: | 
  <p>Jen Kane is an entrepreneur, yoga instructor, health and wellness advocate, and life coach.</p>
  <p>We worked together to create a logo, brand identity, and style guide for her personal brand that reflects her fun-loving personality. </p>
order: 4
image: /assets/clients/jen-kane/jen1.jpg
---


<div class="grid client-images">
	{% for image in site.static_files %}
	    {% if image.path contains '/clients/jen-kane' %}
		    {% assign mod = forloop.index | modulo: 2 %}
		    {% if mod == 0 %}
		    	<div class="grid__item medium-up--one-half">
		        	<img src="{{ site.baseurl }}{{ image.path }}" alt="Pioneer Craft House video"/>
		        </div>
		    {% else %}
		    	<div class="grid__item medium-up--one-half">
		        	<img src="{{ site.baseurl }}{{ image.path }}" alt="Pioneer Craft House video"/>
		        </div>
		    {% endif %}
	    {% endif %}
	{% endfor %}
</div>