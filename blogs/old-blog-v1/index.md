---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>My very first blog</h2>
		Developed in 30min during a lecture
	</section>
	<section>
			<table>
			{% for post in site.categories.old-blog-v1 %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>