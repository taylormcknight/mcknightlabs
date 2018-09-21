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
		{% for tech-design in site.categories.tech-design %}
		<article>
			<figcaption>
				{% if tech-design.external_url %}
				<a href="{{ tech-design.external_url }}">
				{% else %}
				<a href="{{ tech-design.url }}">
				{% endif %}
				<h3>
					{{ tech-design.title }}
				</h3>
				</a>
				<p>{{ tech-design.date | date: "%-d %B %Y" }}</p>
				<p class="description">{{ tech-design.description }}</p>
				{% if tech-design.external_url %}
				<a href="{{ tech-design.external_url }}">
				{% else %}
				<a href="{{ tech-design.url }}">
				{% endif %}
				<p class="meta">Read more</p>
				</a>
			</figcaption>
			{% if tech-design.image %}
			<figure>
				{% if tech-design.external_url %}
				<a href="{{ tech-design.external_url }}">
				{% else %}
				<a href="{{ tech-design.url }}">
				{% endif %}
				<img src="{{ tech-design.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>
