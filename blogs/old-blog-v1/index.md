---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>My very first blog</h2>
		<p>Developed in 30min during a lecture</p>
		<img src="screenshot.png" width="240" style="border: 1px solid #000; padding: 2px;" /><br/>
		<small><em>Screenshot</em></small>
	</section>
	<section>
		<h4>Archived entries</h4>
		<table>
			{% for post in site.categories.old-blog-v1 %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
		</table>
	</section>
</div>