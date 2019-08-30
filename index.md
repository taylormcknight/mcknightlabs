---
layout: full-width
title: R. Taylor McKnight
description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_title: R. Taylor McKnight
og_description: Everything around us was made up by people that were no smarter than us, and we can change it.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<nav class="top-nav-desktop">
	<a href="{{ site.url }}" class="logo">McKnight</a>
	<ul class="nav">
		<li>
			<a href="{{ site.url }}/essays" {% if page.url == '/essays' %}class="current"{% endif %}>Essays</a>
		</li>
		<li>
			<a href="{{ site.url }}/startup" {% if page.url == '/startup' %}class="current"{% endif %}>Startup Journal</a>
		</li>
		<li>
			<a href="{{ site.url }}/design" {% if page.url == '/design' %}class="current"{% endif %}>Personal Projects</a>
		</li>
		<li>
			<a href="{{ site.url }}/goals" {% if page.url == '/goals' %}class="current"{% endif %}>Self-mastery</a>
		</li>
		<li>
			<a href="{{ site.url }}/about" class="{% if page.url == '/about' %}current{% endif %}">About</a>
		</li>
	</ul>
	<div id="myNav" class="overlay">
		<!-- Button to close the overlay navigation -->
		<a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
		<!-- Overlay content -->
		<div class="overlay-content">
			<a href="{{ site.url }}/essays">Essays</a>
			<a href="{{ site.url }}/startup">Startup Journal</a>
			<a href="{{ site.url }}/design">Personal Projects</a>
			<a href="{{ site.url }}/goals">Self-mastery</a>
			<a href="{{ site.url }}/about">About</a>
		</div>
	</div>
	<span onclick="openNav()" class="mobile-menu-btn logo">&#9776;</span>
</nav>
<section class="">
	<section class="grid page-header">
		<div class="full-width">
			<h1>{{ page.title }}
			</h1>
			<p>I am VP of Design at <a href="https://www.industrydive.com/">Industry Dive</a>, where I started in 2013 as <a href="{{ site.baseurl }}{% link _posts/startup/2018-02-05-startupjob.md %}">employee #5</a>.</p>
			<p>View my team's work at <a href="https://industrydive.design/">IndustryDive.design</a>.</p>
			<p>Get in touch <a href="https://twitter.com/rtaylormcknight">@rtaylormcknight</a>.</p>
		</div>
	</section>
</section>
<!--
<section class="grid">
	<div class="full-width">
	</div>
</section>

<!--
<section class="stripe-section-2">
	<section class="grid sub-section-header">
		<div class="full-width">
			<h2>Space</h2>
		</div>
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


</section>-->