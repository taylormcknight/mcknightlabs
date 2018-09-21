---
layout: article
title: Download imagery directly from NOAA satellites for under $30
description: While volunteering with Mach30, a DC-area non-profit committed to open-source space exploration, I used a cheap digital antenna and open-source software to listen to and download data from a number of satellites.
category: experiment
image: https://s3.amazonaws.com/rtmup.com/blog_images/hab/hab_gear.jpg
---

<h3>Hardware required</h3>

<ul>
	<li><a href="http://www.nooelec.com/store/sdr/sdr-receivers/nesdr-mini2-rtl2832u-r820t2.html">SDR USB</a> + antenna</li>
	<li>Mac or Linux Laptop</li>
</ul>

<h3>Software required</h3>

<table>
	<tr>
		<td>
			<strong>Description</strong>
		</td>
		<td>
			<strong>OS X Software</strong>	
		</td>
		<td>
			<strong>Linux Software</strong>
		</td>
	</tr>
	<tr>
		<td>
			Software Receiver
		</td>
		<td>
			<a href="http://cubicsdr.com/">CubicSDR</a>	
		</td>
		<td>
			<a href="http://cubicsdr.com/">CubicSDR</a>
		</td>
	</tr>
	<tr>
		<td>
			Audio Capture Tool
		</td>
		<td>
			<a href="http://www.audacityteam.org/">Audacity</a>	
		</td>
		<td>
			<a href="http://www.audacityteam.org/">Audacity</a>
		</td>
	</tr>
	<tr>
		<td>
			Audio Router
		</td>
		<td>
			<a href="http://rogueamoeba.com/freebies/soundflower/">Soundflower</a>	
		</td>
		<td>
			<a href="https://www.freedesktop.org/wiki/Software/PulseAudio/">PulseAudio</a>
		</td>
	</tr>
	<tr>
		<td>
			Satellite Pass Predictor
		</td>
		<td>
			<a href="https://itunes.apple.com/us/app/satsat/id1017063968?ls=1&mt=8">SatSat</a> or <a href="http://gpredict.oz9aec.net/">GPredict</a>
		</td>
		<td>
			<a href="https://itunes.apple.com/us/app/satsat/id1017063968?ls=1&mt=8">SatSat</a> or <a href="http://gpredict.oz9aec.net/">GPredict</a>
		</td>
	</tr>
	<tr>
		<td>
			Image Processor
		</td>
		<td>
			<a href="http://www.wxtoimg.com/">WXtoImg</a>
		</td>
		<td>
			<a href="http://www.wxtoimg.com/">WXtoImg</a>
		</td>
	</tr>
</table>

<h3>Step 1: Get set up to receive radio signals</h3>

<p>Download CubicSDR.</p>
<p>Connect the antenna to the Nooelec and the Nooelec to your laptop.</p>
<p>Open CubicSDR. File > SDR Devices. Then select your SDR device under "local" and click the "add remote" button.</h3>
<p>Set the frequency to a local radio station.</p>

<h3>Step 2: Tune into a NOAA satellite frequency</h3>

<p>NOAA-15

<h3>Step 3: Auto-record NOAA satellite images</h3>


