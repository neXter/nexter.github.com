---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>San Francisco 2013</h2>
		16.03. bis 29.3. 2013, erst 1 Woche Urlaub, danach eine Woche auf der GDC.
	</section>
	<section>
			<table>
			{% for post in site.categories.sfo-2013 %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
			</table>
	</section>
</div>