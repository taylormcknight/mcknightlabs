---
layout: full-width
title: Business
description: Reflections on my startup and business experiences
og_title: Startup Journal | Taylor McKnight
og_description: Reflections on my startup and business experiences
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid page-header">
	<div class="full-width">
		<h1>{{ page.title }}</h1>
		<p>Reflections on my startup and business experiences</p>
	</div>
</section>
<section class="stripe-section-2">
	<section class="grid-wrapper feed">
		{% for startup in site.categories.startup %}
		<article>
			<figcaption>
				{% if startup.external_url %}
				<a href="{{ startup.external_url }}">
				{% else %}
				<a href="{{ startup.url }}">
				{% endif %}
				<h3>
					{{ startup.title }}
				</h3>
				</a>
				<p class="label">{{ startup.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ startup.description }}</p>
				<p>
				{% if startup.external_url %}
				<a href="{{ startup.external_url }}">
				{% else %}
				<a href="{{ startup.url }}">
				{% endif %}
				Read more
				</a>
				</p>
			</figcaption>
			{% if startup.image %}
			<figure>
				{% if startup.external_url %}
				<a href="{{ startup.external_url }}">
				{% else %}
				<a href="{{ startup.url }}">
				{% endif %}
				<img src="{{ startup.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>
