---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>San Francisco 2013</h2>
		1 week vacation + GDC 2013
	</section>
	<section>
			<table>
			{% for post in site.categories.sfo-2013 %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>