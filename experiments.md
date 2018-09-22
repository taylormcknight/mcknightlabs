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
		<h1>{{ page.title }}</h1>
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
				<a href="{{ experiment.url }}"><p class="meta">Read more</p></a>
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