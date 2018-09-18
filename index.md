---
layout: full-width
title: Ryan McKnight
description: I founded and lead the award-winning design team at Industry Dive, a rapidly growing business news company in Washington, DC.
og_title: Ryan McKnight, Head of Design
og_description: I founded and lead the award-winning design team at Industry Dive, a rapidly growing business news company in Washington, DC.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid">
<article>
<h1>{{ page.title }}</h1>

<p>I founded and lead the multidisciplinary and <a href="https://www.industrydive.com/news/post/honoring-industry-dives-award-winning-design-leader/">award-winning</a> <a href="https://design.industrydive.com/">design team</a> at <a href="https://www.industrydive.com/">Industry Dive</a>, a rapidly growing business news company in Washington, DC. We were selected a "Best Place to Work" by the Washington Post in 2017 and 2018.</p>

<p>In 2017, I was recognized as an "<a href="http://www.siia.net/bims/SPECIAL-PROGRAMS/Emerging-Leader-Awards">Emerging Leader</a>" in the B2B media industry for my work at Industry Dive.</p>

<p>I joined the Industry Dive team during year one and became <a href="{{ site.url }}/tech/2018/02/05/startupjob">FTE #5</a>. Within five years, we scaled the company to over 100 FTEs and $15M+ in annual revenue.</p>

<p>Read about my startup and management experiences <a href="{{ site.url }}/tech-design">here</a>.</p>

<p><strong>Get in touch.</strong></p>
<p>Direct message me on <a href="https://www.twitter.com/mcknightlabs">Twitter</a>, <a href="https://www.instagram.com/mountainlogbook
">Instagram</a> or <a href="https://www.linkedin.com/in/ryantmcknight/">LinkedIn</a>.</p>

<p><strong>Self-mastery is what drives me.</strong> Check out my personal projects below.</p>
</article>
</section>
<section class="stripe-section">
	<section class="gallery">
		{% for page in site.activities %}
		<article>
			<figcaption>
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				{% endif %}
				<h3>
					{{ page.title }}
				</h3>
				</a>
				<p class="description">{{ page.description }}</p>
				<!--<a href="{{ page.url }}"><p class="meta">Read more</p></a>-->
			</figcaption>
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
		</article>
		{% endfor %}
	</section>
</section>