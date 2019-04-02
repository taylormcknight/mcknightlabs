---
layout: full-width
title: Personal Projects
description: Health and wellbeing design projects
og_title: Personal Projects | Ryan McKnight
og_description: Health and wellbeing design projects
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid page-header">
	<div class="full-width">
		<h1>{{ page.title }}</h1>
		<p>Health and wellbeing design projects</p>
	</div>
</section>

<section class="stripe-section-2">
	<section class="grid-wrapper tiles">
		{% assign healthprojects = site.projects | where: "category", "health" | sort:"weight" %}
		{% for page in healthprojects %}
		<article>
			<figure>
				{% if page.image %}
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<img src="{{ page.image }}" />
				</a>
				{% endif %}
				<figcaption>
					{% if page.external_url %}
					<a href="{{ page.external_url }}">
					{% else %}
					<a href="{{ page.url }}">
					{% endif %}
					{% if page.label %}
					<p class="label">{{ page.label }}</p>
					{% endif %}
					<h3>
						{{ page.title }}
					</h3>
					</a>
					<p>
					{{ page.description }}
					</p>
					<p>
					{% if page.external_url %}
					<a href="{{ page.external_url }}">
					{% else %}
					<a href="{{ page.url }}">
					Read more
					{% endif %}
					</a>
					</p>
				</figcaption>
			</figure>
		</article>
		{% endfor %}
	</section>
</section>
<!--
<section class="grid-wrapper tiles">
	{% assign spaceprojects = site.projects | where: "category", "space" | sort:"weight" %}
	{% for page in spaceprojects %}
	<article>
		<figure>
			{% if page.image %}
			{% if page.external_url %}
			<a href="{{ page.external_url }}">
			{% else %}
			<a href="{{ page.url }}">
			{% endif %}
			<img src="{{ page.image }}" />
			</a>
			{% endif %}
			<figcaption>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				{% if page.label %}
				<p class="label">{{ page.label }}</p>
				{% endif %}
				<h3>
					{{ page.title }}
				</h3>
				</a>
				<p>
				{{ page.description }}
				</p>
				<p>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				Read more
				{% endif %}
				</a>
				</p>
			</figcaption>
		</figure>
	</article>
	{% endfor %}
</section>-->