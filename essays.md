---
layout: full-width
title: Essays
description: Experiences and lessons I have learned
og_title: Essays | Ryan McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid page-header">
	<div class="full-width">
		<h1>{{ page.title }}</h1>
		<p>Thoughts on wellbeing and longevity</p>
	</div>
</section>
<section class="stripe-section-2">
	<section class="grid-wrapper feed">
		{% for essay in site.categories.essay %}
		<article>
			<figcaption>
				{% if essay.external_url %}
				<a href="{{ essay.external_url }}">
				{% else %}
				<a href="{{ essay.url }}">
				{% endif %}
				<h3>
					{{ essay.title }}
				</h3>
				</a>
				<p class="label">{{ essay.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ essay.description }}</p>
				<p>
				{% if essay.external_url %}
				<a href="{{ essay.external_url }}">
				{% else %}
				<a href="{{ essay.url }}">
				{% endif %}
				Read more
				</a>
				</p>
			</figcaption>
			{% if essay.image %}
			<figure>
				{% if essay.external_url %}
				<a href="{{ essay.external_url }}">
				{% else %}
				<a href="{{ essay.url }}">
				{% endif %}
				<img src="{{ essay.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>
