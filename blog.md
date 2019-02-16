---
layout: full-width
title: Blog
description: Experiences and lessons I have learned
og_title: Portfolio | Ryan McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="stripe-section">
	<section class="grid page-header">
		<div class="full-width">
			<h1>{{ page.title }}</h1>
			<p>Thoughts on tech and design by <a href="https://twitter.com/ryantmcknight">@RyanTMcKnight</a></p>
		</div>
	</section>
</section>
<section class="stripe-section-2">
	<section class="grid-wrapper feed">
		{% for blog in site.categories.blog %}
		<article>
			<figcaption>
				{% if blog.external_url %}
				<a href="{{ blog.external_url }}">
				{% else %}
				<a href="{{ blog.url }}">
				{% endif %}
				<h3>
					{{ blog.title }}
				</h3>
				</a>
				<p class="label">{{ blog.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ blog.description }}</p>
				<p>
				{% if blog.external_url %}
				<a href="{{ blog.external_url }}">
				{% else %}
				<a href="{{ blog.url }}">
				{% endif %}
				Read more
				</a>
				</p>
			</figcaption>
			{% if blog.image %}
			<figure>
				{% if blog.external_url %}
				<a href="{{ blog.external_url }}">
				{% else %}
				<a href="{{ blog.url }}">
				{% endif %}
				<img src="{{ blog.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>
