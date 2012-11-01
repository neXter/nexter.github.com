---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>Living in WoW</h2>
		Meine Beiträge zu einem Blog rund um World of Warcraft in den Jahren 2005 bis 2007
	</section>
	<section>
			<table>
			{% for post in site.categories.living-in-wow %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>