---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>blog.2sekunden.net</h2>
		Based on Tumblr
	</section>
	<section>
		<table>
			{% for post in site.categories.tumblr %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
		</table>
	</section>
</div>