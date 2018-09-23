---
layout: full-width
title: Portfolio
description: Ryan McKnight founded and leads the award-winning design team at Industry Dive, a rapidly growing business news company in Washington, DC.
og_title: Portfolio | Ryan McKnight
og_description: Ryan McKnight founded and leads the award-winning design team at Industry Dive, a rapidly growing business news company in Washington, DC.
og_image: /media/img/about/mcknight_headshot.jpg
og_type: website
---
<section class="grid">
	<article>
		<h1>{{ page.title }}</h1>
		<!--<p>The most important part of my job as a manager and team leader is shepherding the best ideas of my employees to fruition. I also work hard to align the personal interests and skills of my team members with core needs of the business to push the needle forward.</p>
		<p>For a closer look at my growth as a manager, read <a href="{{ site.baseurl }}{% link _posts/blog/2017-03-05-management.md %}">this post</a>.</p>-->
		<p>After graduating from LSE in 2012, I joined Industry Dive as employee #5, taught myself the fundamentals of design and front-end development and built a team of designers. I also founded the following areas of design and multi-media at the company: <a href="https://design.industrydive.com/ux/2018/01/04/cms-audit-user-flows.html">UX design</a>, <a href="https://design.industrydive.com/product/2017/12/20/library-page.html">UI design</a>, <a href="https://design.industrydive.com/product/2018/03/29/flex-menu.html">front-end development</a>, <a href="https://design.industrydive.com/editorial/2018/03/08/dive-awards-2017.html">editorial graphics</a>, podcasting, <a href="https://www.constructiondive.com/news/photos-of-new-smithsonian-african-american-museum/420671/">photo journalism</a> and <a href="https://design.industrydive.com/corporate/2018/05/09/logo-redesign.html">graphic design</a>.</p>
		<p> On nights and weekends, I worked as a UI/UX consultant for a <a href="https://lyflynks.com/">healthcare startup</a> in the caregiving space and helped my barber launch a <a href="https://www.callfigaro.com/">mobile salon</a> in DC.</p>
		<p>Learn about a few of my projects below.</p>
	</article>
</section>
<section class="stripe-section">
	<section class="grid-wrapper">
		{% for page in site.projects %}
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
				{% if page.external_url %}
				<a href="{{ page.external_url }}">
				{% else %}
				<a href="{{ page.url }}">
				<p class="meta">Read more</p>
				{% endif %}
				</a>
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
<!--
	<h2>Corporate branding</h2> 

	<h2>Editorial design/h2> 
	
	<h2>Company leadership</h2> 
	
			
	<div class="medium-frame tweet-feed">
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Our <a href="https://twitter.com/divedesigners?ref_src=twsrc%5Etfw">@divedesigners</a> are in the planning phase of a CMS redesign. Very cool to watch the process! 💻💡 <a href="https://t.co/rfC6nIxvuo">pic.twitter.com/rfC6nIxvuo</a></p>&mdash; Industry Dive (@industrydive) <a href="https://twitter.com/industrydive/status/900445325219037185?ref_src=twsrc%5Etfw">August 23, 2017</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">&quot;Auditing our CMS and creating user flow diagrams&quot; by <a href="https://twitter.com/nforman44?ref_src=twsrc%5Etfw">@nforman44</a> <a href="https://t.co/xo6ZVM60xv">https://t.co/xo6ZVM60xv</a> <a href="https://twitter.com/hashtag/design?src=hash&amp;ref_src=twsrc%5Etfw">#design</a> <a href="https://twitter.com/hashtag/ux?src=hash&amp;ref_src=twsrc%5Etfw">#ux</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/966064824793878531?ref_src=twsrc%5Etfw">February 20, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Our email newsletters are now 33% smaller in file size and optimized for more clients thanks to <a href="https://twitter.com/nforman44?ref_src=twsrc%5Etfw">@nforman44</a>. How did she accomplish this? Find out in this post: <a href="https://t.co/Cd96U2Ghbl">https://t.co/Cd96U2Ghbl</a> <a href="https://twitter.com/hashtag/design?src=hash&amp;ref_src=twsrc%5Etfw">#design</a> <a href="https://twitter.com/hashtag/tech?src=hash&amp;ref_src=twsrc%5Etfw">#tech</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/976204524024160259?ref_src=twsrc%5Etfw">March 20, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">&quot;Creating downloadable PDFs using the .print window&quot; by <a href="https://twitter.com/nancopeland?ref_src=twsrc%5Etfw">@nancopeland</a> <a href="https://t.co/69lUWTWmK9">https://t.co/69lUWTWmK9</a> <a href="https://twitter.com/hashtag/frontend?src=hash&amp;ref_src=twsrc%5Etfw">#frontend</a> <a href="https://twitter.com/hashtag/design?src=hash&amp;ref_src=twsrc%5Etfw">#design</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/971047466866012160?ref_src=twsrc%5Etfw">March 6, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">A little <a href="https://twitter.com/hashtag/FlashbackFriday?src=hash&amp;ref_src=twsrc%5Etfw">#FlashbackFriday</a>: Evolution of our sites over the past 3 years. Our redesign is 🔥 thanks to <a href="https://twitter.com/rtmup?ref_src=twsrc%5Etfw">@rtmup</a> &amp; our design team! <a href="https://t.co/GOZjZj9zmD">pic.twitter.com/GOZjZj9zmD</a></p>&mdash; Industry Dive (@industrydive) <a href="https://twitter.com/industrydive/status/786939466875342849?ref_src=twsrc%5Etfw">October 14, 2016</a></blockquote>
		</figure>
	</div>

	<h2>Corporate Branding</h2>
	<div class="medium-frame tweet-feed">
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">An openness to bottom-up ideas is one of our company&#39;s greatest strengths. The year-long process to redesign our logo was sparked by a proposal from a handful of employees, not management or the founders. <a href="https://t.co/JpEF7beVP7">https://t.co/JpEF7beVP7</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/973914961717194752?ref_src=twsrc%5Etfw">March 14, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Check out this behind-the-scenes post on our logo redesign by <a href="https://twitter.com/KDesigning?ref_src=twsrc%5Etfw">@KDesigning</a> and <a href="https://twitter.com/elizam0075?ref_src=twsrc%5Etfw">@elizam0075</a> <a href="https://t.co/45wFl2aRlR">https://t.co/45wFl2aRlR</a> <a href="https://twitter.com/hashtag/design?src=hash&amp;ref_src=twsrc%5Etfw">#design</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/994670275714342912?ref_src=twsrc%5Etfw">May 10, 2018</a></blockquote>
		</figure>
	</div>

	<h2>Editorial design</h2>
	<div class="medium-frame tweet-feed">
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Shout out to <a href="https://twitter.com/Jordan_EBranch?ref_src=twsrc%5Etfw">@Jordan_EBranch</a> for designing this piece on women in the power sector. Also to <a href="https://twitter.com/elizam0075?ref_src=twsrc%5Etfw">@elizam0075</a> for the really fun illustrations! <a href="https://twitter.com/divedesigners?ref_src=twsrc%5Etfw">@divedesigners</a> <a href="https://t.co/AMWJX8TEST">https://t.co/AMWJX8TEST</a></p>&mdash; Natalie Forman (@nforman44) <a href="https://twitter.com/nforman44/status/985959023290798081?ref_src=twsrc%5Etfw">April 16, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Check out these new editorial illustrations by our highly talented graphic design intern and recent <a href="https://twitter.com/risd?ref_src=twsrc%5Etfw">@risd</a> grad, Yujin Kim. <a href="https://t.co/6r82D4jyZu">pic.twitter.com/6r82D4jyZu</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/1012697550233587713?ref_src=twsrc%5Etfw">June 29, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">What is involved in leading a major editorial design project? Read about <a href="https://twitter.com/Jordan_EBranch?ref_src=twsrc%5Etfw">@Jordan_EBranch</a>&#39;s experience with the 2017 Dive Awards: <a href="https://t.co/KYq0tH4Sd9">https://t.co/KYq0tH4Sd9</a> <a href="https://twitter.com/hashtag/design?src=hash&amp;ref_src=twsrc%5Etfw">#design</a> <a href="https://twitter.com/hashtag/journalism?src=hash&amp;ref_src=twsrc%5Etfw">#journalism</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/976208311451291650?ref_src=twsrc%5Etfw">March 20, 2018</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">&quot;What Chinese import policies mean for all 50 states&quot; New visual feature story designed by <a href="https://twitter.com/Jordan_EBranch?ref_src=twsrc%5Etfw">@Jordan_EBranch</a> <a href="https://twitter.com/divedesigners?ref_src=twsrc%5Etfw">@divedesigners</a> <a href="https://t.co/EKg142QB4K">https://t.co/EKg142QB4K</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/930913945111711744?ref_src=twsrc%5Etfw">November 15, 2017</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Our most recent interactive graphics project – &quot;The shifting state of federal CIOs&quot;<a href="https://t.co/CtMJTFhmOF">https://t.co/CtMJTFhmOF</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/926158878097772550?ref_src=twsrc%5Etfw">November 2, 2017</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Amazing work by <a href="https://twitter.com/RetailDive?ref_src=twsrc%5Etfw">@RetailDive</a> and <a href="https://twitter.com/divedesigners?ref_src=twsrc%5Etfw">@divedesigners</a> producing exclusive in-depth interview w/ fascinating character <a href="https://t.co/n3M9d9Ketg">https://t.co/n3M9d9Ketg</a></p>&mdash; Industry Dive (@industrydive) <a href="https://twitter.com/industrydive/status/879373680459091968?ref_src=twsrc%5Etfw">June 26, 2017</a></blockquote>
		</figure>
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Creative Director <a href="https://twitter.com/rtmup?ref_src=twsrc%5Etfw">@rtmup</a> teaching us the Rule of Thirds at our Intro to iPhone Photography brown bag lunch. 📱📸👀 <a href="https://t.co/ievQA4YuX3">pic.twitter.com/ievQA4YuX3</a></p>&mdash; Industry Dive (@industrydive) <a href="https://twitter.com/industrydive/status/840249993659351040?ref_src=twsrc%5Etfw">March 10, 2017</a></blockquote>
		</figure>
	</div>

	<h2>Brand Studio Design</h2>
	<div class="medium-frame tweet-feed">
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">5 awards for <a href="https://twitter.com/industrydive?ref_src=twsrc%5Etfw">@industrydive</a>. 2017 American Graphic Design Awards <a href="https://twitter.com/hashtag/gdusa?src=hash&amp;ref_src=twsrc%5Etfw">#gdusa</a> <a href="https://t.co/ePeAv9NAlI">pic.twitter.com/ePeAv9NAlI</a></p>&mdash; Dive Design Team (@divedesigners) <a href="https://twitter.com/divedesigners/status/921487568860073984?ref_src=twsrc%5Etfw">October 20, 2017</a></blockquote>
		</figure>
	</div>
		
	<h2>Company Leadership</h2>
	<div class="medium-frame tweet-feed">
		<figure>
			<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Proud to be named #5 on <a href="https://twitter.com/washingtonpost?ref_src=twsrc%5Etfw">@washingtonpost</a>&#39;s <a href="https://twitter.com/hashtag/TopWorkplacesDC?src=hash&amp;ref_src=twsrc%5Etfw">#TopWorkplacesDC</a> 🏆and the youngest company across all categories! <a href="https://t.co/Itlc0ECe9D">https://t.co/Itlc0ECe9D</a> <a href="https://t.co/8JtCwbgevN">pic.twitter.com/8JtCwbgevN</a></p>&mdash; Industry Dive (@industrydive) <a href="https://twitter.com/industrydive/status/875730868513513472?ref_src=twsrc%5Etfw">June 16, 2017</a></blockquote>
		</figure>
	</div>
</section>	

	<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
	-->
