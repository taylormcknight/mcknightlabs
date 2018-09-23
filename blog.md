---
layout: full-width
title: Blog
description: Experiences and lessons I have learned
og_title: Portfolio | Ryan McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid">
	<article>
		<h1>{{ page.title }}</h1>
		<p>Reflection is a key element of personal and professional growth, so I blog about experiences and lessons learned. Looking for my more imaginative "what if" posts? Go <a href="{{ site.url }}">here</a>.</p>
	</article>
</section>
<section class="stripe-section">
	<section class="grid-wrapper">
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
				<p>{{ blog.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ blog.description }}</p>
				{% if blog.external_url %}
				<a href="{{ blog.external_url }}">
				{% else %}
				<a href="{{ blog.url }}">
				{% endif %}
				<p class="meta">Read more</p>
				</a>
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