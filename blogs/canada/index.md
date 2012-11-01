---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>Canada 2009</h2>
		Backpacking for four weeks
	</section>
	<section>
			<table>
			{% for post in site.categories.canada %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>