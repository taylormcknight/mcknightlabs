---
layout: full-width
title: Activities
description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_title: Portfolio | Taylor McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="stripe-section">
	<section class="grid-wrapper">
		{% for activity in site.categories.activities %}
		<article>
			<figcaption>
				{% if activity.external_url %}
				<a href="{{ activity.external_url }}">
				{% else %}
				<a href="{{ activity.url }}">
				{% endif %}
				<h3>
					{{ activity.title }}
				</h3>
				</a>
				<p class="description">{{ activity.description }}</p>
				{% if activity.external_url %}
				<a href="{{ activity.external_url }}">
				{% else %}
				<a href="{{ activity.url }}">
				{% endif %}
				<p class="meta">Read more</p>
				</a>
			</figcaption>
			{% if activity.image %}
			<figure>
				{% if activity.external_url %}
				<a href="{{ activity.external_url }}">
				{% else %}
				<a href="{{ activity.url }}">
				{% endif %}
				<img src="{{ activity.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>