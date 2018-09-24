---
layout: full-width
title: Rethinking our world
description: Everything around us was made up by people that were no smarter than us, and we can change it.
image: https://s3.amazonaws.com/rtmup.com/blog_images/hab/stratosphere_5.jpg
og_title: McKnight Labs
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: https://s3.amazonaws.com/rtmup.com/blog_images/hab/stratosphere_5.jpg
og_type: website
---
<section class="grid">
	<div class="full-width">
		<h1>{{ page.title }}</h1>
		<p>Everything around us was made up by people that were no smarter than us, and we can change it.</p>
	</div>
</section>
<section class="stripe-section">
	<section class="grid-wrapper">
		{% for rethinking in site.categories.rethinking %}
		<article>
			<figcaption>
				{% if rethinking.external_url %}
				<a href="{{ rethinking.external_url }}">
				{% else %}
				<a href="{{ rethinking.url }}">
				{% endif %}
				<h3>
					{{ rethinking.title }}
				</h3>
				</a>
				<p>{{ rethinking.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ rethinking.description }}</p>
				<p>
				{% if rethinking.external_url %}
				<a href="{{ rethinking.external_url }}">
				{% else %}
				<a href="{{ rethinking.url }}">
				{% endif %}
				Read more
				</a>
				</p>
			</figcaption>
			{% if rethinking.image %}
			<figure>
				{% if rethinking.external_url %}
				<a href="{{ rethinking.external_url }}">
				{% else %}
				<a href="{{ rethinking.url }}">
				{% endif %}
				<img src="{{ rethinking.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>