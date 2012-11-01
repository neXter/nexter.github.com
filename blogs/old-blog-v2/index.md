---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>Second iteration of my personal blog</h2>
		Small upgrade over previous one, still self coded
	</section>
	<section>
			<table>
			{% for post in site.categories.old-blog-v2 %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>