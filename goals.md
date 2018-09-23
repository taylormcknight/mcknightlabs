---
layout: full-width
title: Goals
description: We become the things we do
og_title: Goals | Ryan McKnight
og_description: We become the things we do
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid">
	<article>
		<h1>{{ page.title }}</h1>
		<p>We become the things we do. Self-mastery is what drives me. Below are personal goals I have achieved.</p>
	</article>
</section>
<section class="stripe-section">
	<section class="grid-wrapper">
		{% for goal in site.categories.goal %}
		<article>
			<figcaption>
				{% if goal.external_url %}
				<a href="{{ goal.external_url }}">
				{% else %}
				<a href="{{ goal.url }}">
				{% endif %}
				<h3>
					{{ goal.title }}
				</h3>
				</a>
				<p class="description">{{ goal.description }}</p>
				<p>
				{% if goal.external_url %}
				<a href="{{ goal.external_url }}">
				{% else %}
				<a href="{{ goal.url }}">
				{% endif %}
				Read more
				{% if goal.external_url %}
				<img src="{{ site.url }}/media/img/external-link-icon.png" class="external-link-icon">
				{% endif %}
				</a>
				</p>
			</figcaption>
			{% if goal.image %}
			<figure>
				{% if goal.external_url %}
				<a href="{{ goal.external_url }}">
				{% else %}
				<a href="{{ goal.url }}">
				{% endif %}
				<img src="{{ goal.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>