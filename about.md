---
layout: full-width
title: About Ryan
description: I founded and lead the award-winning design team at Industry Dive, a rapidly growing business news company in Washington, DC.
og_title: Ryan McKnight, Head of Design
og_description: I founded and lead the award-winning design team at Industry Dive, a rapidly growing business news company in Washington, DC.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="stripe-section">
<section class="inner-section-wrapper">

<h1>{{ page.title }}</h1>

<img src="/media/img/about/mcknight.jpg" class="headshot">

<p>I founded and lead the multidisciplinary and <a href="https://www.industrydive.com/news/post/honoring-industry-dives-award-winning-design-leader/">award-winning</a> <a href="https://design.industrydive.com/">design team</a> at <a href="https://www.industrydive.com/">Industry Dive</a>, a business journalism startup in Washington, D.C.</p> 

<p>In 2018, Industry Dive appeared on <em>Inc.</em> magazine's list of <a href="https://www.industrydive.com/news/post/inc-names-industry-dive-one-of-the-fastest-growing-private-companies-in-america/">fastest-growing private companies in America</a>. The company was also recognized as a "<a href="https://www.industrydive.com/news/post/industry-dive-honored-as-top-workplace-and-red-hot-company/">Best Place to Work</a>" in DC by the Washington Post in 2017 and 2018.</p>

<h2>Get in touch</h2>

<p>Direct message me on <a href="https://www.twitter.com/ryantmcknight">Twitter</a>, <a href="https://www.instagram.com/mountainlogbook
">Instagram</a> or <a href="https://www.linkedin.com/in/ryantmcknight/">LinkedIn</a>.</p>

<h2>Full bio</h2>

<p>After graduating from <a href="http://www.lse.ac.uk/">LSE</a> in 2012, I joined <a href="https://www.industrydive.com/">Industry Dive</a>, a business journalism startup, as <a href="{{ site.url }}/blog/2018/02/05/startupjob">employee #5</a> and taught myself the fundamentals of design and front-end development.</p>

<p>I founded the following areas of design and multi-media at Industry Dive: <a href="https://design.industrydive.com/ux/2018/01/04/cms-audit-user-flows.html">UX design</a>, <a href="https://design.industrydive.com/product/2017/12/20/library-page.html">UI design</a>, <a href="https://design.industrydive.com/product/2018/03/29/flex-menu.html">(agile) front-end development</a>, <a href="https://design.industrydive.com/editorial/2018/03/08/dive-awards-2017.html">editorial graphics</a>, <a href="https://www.constructiondive.com/news/photos-of-new-smithsonian-african-american-museum/420671/">photo journalism</a> and <a href="https://design.industrydive.com/corporate/2018/05/09/logo-redesign.html">graphic design</a>.</p>

<p>Within six years, I built an eight-person multidisciplinary <a href="https://design.industrydive.com/">design team</a> that won 8 <a href="https://www.industrydive.com/news/post/honoring-industry-dives-award-winning-design-leader/">American Graphic Design Awards</a> and helped scale the company to over 100 FTEs and $15M+ in revenue.</p>

<p>In 2017, I was recognized as an "<a href="http://www.siia.net/bims/SPECIAL-PROGRAMS/Emerging-Leader-Awards">Emerging Leader</a>" in the B2B media industry for my work at Industry Dive and, in 2018, served as a judge in the same <a href="https://www.siia.net/bims/SPECIAL-PROGRAMS/Emerging-Leader-Awards">national awards competition</a>.</p>

<p>Read about my startup and management experiences <a href="{{ site.url }}/blog/2017/03/05/management">here</a>.</p>

<p>On nights and weekends, I have worked as a UI/UX consultant for a <a href="https://lyflynks.com/">healthcare startup</a> in the caregiving space, volunteered with an <a href="http://mach30.org/">open source aerospace group</a> and helped my barber launch a <a href="https://www.callfigaro.com/">mobile salon</a> in DC.</p>

<h2>Self-mastery is what drives me</h2>

<p>I am a scuba diver, freediver, wilderness first aid responder, <a href="http://divegoals.com/uwp/2018/01/30/uwphotography.html">underwater photographer</a> and alpine mountaineer. I have photographed the earth <a href="{{ site.baseurl }}{% link _projects/space/2016-06-24-hab-part-2.md %}">from the stratosphere</a>, marine life in the <a href="http://divegoals.com/dive/2018/01/29/galapagos.html">Galápagos</a> and <a href="https://www.instagram.com/p/BhjlN3wjOvB/?taken-by=divegoals">shipwrecks</a> in the Red Sea. I have also trekked to <a href="http://summitgoals.com/ascents/2016/11/05/everest.html">Everest Base Camp</a> and summited <a href="http://summitgoals.com/ascents/2017/01/12/kilimanjaro.html">Mt. Kilimanjaro</a> and <a href="http://summitgoals.com/ascents/2018/06/21/rainier.html">Mt. Rainier</a>.</p>
<p>Below are personal goals I have achieved.</p>
</section>
</section>
<section class="stripe-section-2">
	<section class="grid-wrapper feed">
		{% for goal in site.categories.goal %}
		<article>
			<figcaption>
				{% if goal.external_url %}
				<a href="{{ goal.external_url }}">
				{% else %}
				<a href="{{ goal.url }}">
				{% endif %}
				<h3>
					{{ goal.title }}
				</h3>
				</a>
				<p class="description">{{ goal.description }}</p>
				<p>
				{% if goal.external_url %}
				<a href="{{ goal.external_url }}">
				{% else %}
				<a href="{{ goal.url }}">
				{% endif %}
				Read more
				{% if goal.external_url %}
				<img src="{{ site.url }}/media/img/external-link-icon.png" class="external-link-icon">
				{% endif %}
				</a>
				</p>
			</figcaption>
			{% if goal.image %}
			<figure>
				{% if goal.external_url %}
				<a href="{{ goal.external_url }}">
				{% else %}
				<a href="{{ goal.url }}">
				{% endif %}
				<img src="{{ goal.image }}" />
				</a>
			</figure>
			{% endif %}
		</article>
		{% endfor %}
	</section>
</section>


<!--I founded and lead the multi-disciplinary and <a href="https://www.industrydive.com/news/post/honoring-industry-dives-award-winning-design-leader/">award-winning</a> <a href="https://design.industrydive.com/">design team</a> at <a href="https://www.industrydive.com/">Industry Dive</a>, a rapidly growing business news company in Washington, DC. We were selected a "Best Place to Work" by the Washington Post in 2017 and 2018.
In 2017, I was recognized as an "<a href="http://www.siia.net/bims/SPECIAL-PROGRAMS/Emerging-Leader-Awards">Emerging Leader</a>" in the B2B media industry for my work at Industry Dive.
To get in touch, direct message me on <a href="https://www.twitter.com/mcknightlabs">Twitter</a>, <a href="https://www.instagram.com/mountainlogbook
">Instagram</a> or <a href="https://www.linkedin.com/in/ryantmcknight/">LinkedIn</a>.-->