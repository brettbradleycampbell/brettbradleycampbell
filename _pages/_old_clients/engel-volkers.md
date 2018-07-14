---
layout: page-client
title: Engel & Völkers
category: 'clients'
services: 
- video
description: | 
  <p>Engel & Völkers' have a beautiful Park City property they needed to showcase.</p>
  <p>Our video focuses on the indoor and outdoor views, to give prospective customers a tangible feeling and sense of the property. </p>

permalink: /clients/engel-volkers
---

<div class="grid client-images">
	{% for image in site.static_files %}
	    {% if image.path contains '/clients/engel-volkers/screenshots' %}
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
<div class="grid">
	<div class="grid__item">
		<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/237455504?title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
	</div>
</div>

