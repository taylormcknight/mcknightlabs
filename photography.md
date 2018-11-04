---
layout: full-width
title: Photography
description: Below are galleries of my film photography. My digital work is focused on the evolution of the earth and can be viewed and purchased <a href="https://scarceart.com/about">here</a>.
og_title: Photography | Ryan McKnight
og_description:
og_image: /media/img/photography/film/35/canonae1/000015350010.jpg
og_type: website
---
<section class="grid page-header">
	<div class="full-width">
		<h1>{{ page.title }}</h1>
		<p>Below are galleries of my film photography. My digital work is focused on the evolution of the earth and can be viewed and purchased on <a href="https://scarceart.com/">ScarceArt.com</a>.</p>
	</div>
</section>
<section class="stripe-section">
	<section class="grid-wrapper">
		{% for page in site.photography %}
		<article>
			<figcaption>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<h3>
					{{ page.title }}
				</h3>
				</a>
				<p class="description">{{ page.description }}</p>
				<p>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				View gallery
				{% endif %}
				</a>
				</p>
			</figcaption>
			{% if page.image %}
			<figure>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<img src="{{ page.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>