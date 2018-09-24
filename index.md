---
layout: full-width
title: Experiments
description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_title: Portfolio | Ryan McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid">
	<article>
	<h1>{{ page.title }}
	<?xml version="1.0" encoding="utf-8"?>
	<!-- Generator: Adobe Illustrator 20.1.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
	<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	viewBox="0 0 92 92" class="page-title-svg" style="enable-background:new 0 0 92 92;" xml:space="preserve">
	<path d="M58.4,65.6c7.4-12.1,15.3-27,15.3-35.2C73.7,15.1,61.3,2.7,46,2.7S18.3,15.1,18.3,30.3c0,8.2,7.9,23.1,15.3,35.2
	c-0.6,0.3-0.9,0.9-0.9,1.6c0,1.1,0.9,1.9,1.9,1.9h2.9c0.5,1.4,0.9,2.8,1.4,4.2c0.7,2.1,1.4,4.2,2,6.3h-1.3c-0.5,0-0.9,0.4-0.9,0.9
	c0,0.5,0.4,0.9,0.9,0.9h0.2l1.7,8h8.9l1.7-8h0.2c0.5,0,0.9-0.4,0.9-0.9c0-0.5-0.4-0.9-0.9-0.9h-1c0.5-1.6,1-3.1,1.5-4.7
	c0.6-1.9,1.2-3.9,1.8-5.8h2.7c1.1,0,1.9-0.9,1.9-1.9C59.3,66.5,58.9,65.9,58.4,65.6z M51.6,74.5c-0.5,1.7-1.1,3.4-1.6,5.1h-7.6
	c-0.7-2.3-1.4-4.5-2.2-6.7c-0.4-1.3-0.8-2.5-1.3-3.8h14.4C52.7,70.9,52.2,72.8,51.6,74.5z"/>
	</svg>
	</h1>
		<p>&ldquo;There are naive questions, tedious questions, ill-phrased questions, questions put after inadequate self-criticism. But every question is a cry to understand the world. There is no such thing as a dumb question.&rdquo; – Carl Sagan</p>
	</article>
</section>
<section class="stripe-section">
	<section class="grid-wrapper">
		{% for experiment in site.categories.experiment %}
		<article>
			<figcaption>
				{% if experiment.external_url %}
				<a href="{{ experiment.external_url }}">
				{% else %}
				<a href="{{ experiment.url }}">
				{% endif %}
				<h3>
					{{ experiment.title }}
				</h3>
				</a>
				<p class="description">{{ experiment.description }}</p>
				<p>
				<a href="{{ experiment.url }}">
				Read more
				</a></p>
			</figcaption>
			{% if experiment.image %}
			<figure>
				{% if experiment.external_url %}
				<a href="{{ experiment.external_url }}">
				{% else %}
				<a href="{{ experiment.url }}">
				{% endif %}
				<img src="{{ experiment.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>