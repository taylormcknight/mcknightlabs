---
layout: full-width
title: Experiments
description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_title: McKnight Labs
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid page-header">
	<div class="full-width">
		<h1>{{ page.title }}
		</h1>
			<p>&ldquo;There are naive questions, tedious questions, ill-phrased questions, questions put after inadequate self-criticism. But every question is a cry to understand the world. There is no such thing as a dumb question.&rdquo; <cite class="page-description-citation">– Carl Sagan, <a href="https://en.wikipedia.org/wiki/The_Demon-Haunted_World">The Demon-Haunted World</a></cite></p>
	</div>
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