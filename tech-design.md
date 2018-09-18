---
layout: full-width
title: Rethinking our world
description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_title: Portfolio | Ryan McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid">
	<article>
		<h1>{{ page.title }}</h1>
		<p>Everything around us was made up by people that were no smarter than us, and we can change it.</p>
	</article>
</section>
<section class="stripe-section">
	<section class="gallery">
		{% for unconventional in site.categories.unconventional %}
		<article>
			<figcaption>
				{% if unconventional.external_url %}
				<a href="{{ unconventional.external_url }}">
				{% else %}
				<a href="{{ unconventional.url }}">
				{% endif %}
				<h3>
					{{ unconventional.title }}
				</h3>
				</a>
				<p>{{ unconventional.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ unconventional.description }}</p>
				{% if unconventional.external_url %}
				<a href="{{ unconventional.external_url }}">
				{% else %}
				<a href="{{ unconventional.url }}">
				{% endif %}
				<p class="meta">Read more</p>
				</a>
			</figcaption>
			{% if unconventional.image %}
			<figure>
				{% if unconventional.external_url %}
				<a href="{{ unconventional.external_url }}">
				{% else %}
				<a href="{{ unconventional.url }}">
				{% endif %}
				<img src="{{ unconventional.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>
