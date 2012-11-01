---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>Personal blog</h2>
		Based on Movable Type
	</section>
	<section>
			<table>
			{% for post in site.categories.old-blog-v3 %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>