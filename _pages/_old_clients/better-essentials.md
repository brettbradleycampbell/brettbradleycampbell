---
layout: page-client
title: Better Essentials
category: 'clients'
services:
- branding
- website (ecommerce)
- graphic design
- advertising 
description: | 
  <p>Better Essentials wanted a fun, colorful brand for their organic essential oils. They also needed on online store. </p>
  <p>We built a custom website on Shopify and developed a brand identity.</p>
permalink: /clients/better-essentials
---

<div class="grid client-images">
	{% for image in site.static_files %}
	    {% if image.path contains '/clients/better-essentials' %}
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

<div class="" style="overflow: hidden;">
	<div class="macbook-wrap">
		<div class="iframe-wrap">
		<iframe class="iframe" src="https://www.betteressentials.com"></iframe>
		</div>
	</div>
</div>