---
layout: full-width
title: Ryan McKnight
description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_title: McKnight Labs
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="stripe-section">
	<section class="grid page-header">
		<div class="full-width">
			<h1>{{ page.title }}
			</h1>
			<p>
			Currently Head of Design and co-leading product management at <a href="https://www.industrydive.com/">Industry Dive</a>
			</p>
		</div>
	</section>
</section>
<section class="stripe-section-2">
	<section class="grid sub-section-header">
		<div class="full-width">
			<h2>Health and wellness</h2>
		</div>
	</section>
	<section class="grid-wrapper tiles">
		{% assign healthprojects = site.projects | where: "category", "health" | sort:"weight" %}
		{% for page in healthprojects %}
		<article>
			{% if page.image %}
			<figure>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<img src="{{ page.image }}" />
				</a>
			</figure>
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
		</article>
		{% endfor %}
	</section>
</section>

<section class="stripe-section-2">
	<section class="grid sub-section-header">
		<div class="full-width">
			<h2>Space</h2>
		</div>
	</section>
	<section class="grid-wrapper tiles">
		{% assign spaceprojects = site.projects | where: "category", "space" | sort:"weight" %}
		{% for page in spaceprojects %}
		<article>
			{% if page.image %}
			<figure>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<img src="{{ page.image }}" />
				</a>
			</figure>
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
		</article>
		{% endfor %}
	</section>
</section>

<section class="stripe-section-2">
	<section class="grid sub-section-header">
		<div class="full-width">
			<h2>Journalism</h2>
		</div>
	</section>
	<section class="grid-wrapper tiles">
		{% assign journalismprojects = site.projects | where: "category", "journalism" | sort:"weight" %}
		{% for page in journalismprojects %}
		<article>
			{% if page.image %}
			<figure>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<img src="{{ page.image }}" />
				</a>
			</figure>
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
		</article>
		{% endfor %}
	</section>


</section>