---
layout: page-client
title: Pioneer Craft House
category: 'clients'
services: 
- video
- art direction
description: | 
  <p>The Pioneer Craft House offers art classes to locals in the Salt Lake City area. They provide professional instruction in arts and crafts like pottery, jewelery making, and leather working. </p>
  <p>We were asked to create a promotional video to showcase the facility and inspire prospective students.</p>
secret-content: 
order: 5
image: /assets/clients/pioneer/screenshots/screenshot7.jpg
---


<div class="grid client-images">
	{% for image in site.static_files %}
	    {% if image.path contains '/clients/pioneer/screenshots' %}
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
		<div style="padding:42.5% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/215262488?title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
	</div>
</div>