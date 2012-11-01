---
layout: default
title: pieter.cc
---

<div id="content">
	<section>
		<h3>Blog posts</h3>
		<table>
			{% for post in site.categories.blog %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
		</table>
	</section>
	<section>
		<table>
			<h3>Old blog content</h3>
			<tr><td><small>200x-200x</small></td><td> &#160; <a href="/blogs/canada/">Canada 2009</a> ({{ site.categories.canada | size }} Posts)</td></tr>
			<tr><td><small>200x-200x</small></td><td> &#160; <a href="/blogs/living-in-wow/">Living in WoW Blog</a> ({{ site.categories.living-in-wow | size }} Posts)</td></tr>
			<tr><td><small>200x-200x</small></td><td> &#160; <a href="/blogs/old-blog-v3/">Old personal blog (v3)</a> ({{ site.categories.old-blog-v3 | size }} Posts)</td></tr>
			<tr><td><small>200x-200x</small></td><td> &#160; <a href="/blogs/old-blog-v2/">Old personal blog (v2)</a> ({{ site.categories.old-blog-v2 | size }} Posts)</td></tr>
			<tr><td><small>200x-200x</small></td><td> &#160; <a href="/blogs/old-blog-v1/">Old personal blog (v1)</a> ({{ site.categories.old-blog-v1 | size }} Posts)</td></tr>
		</table>
	</section>
</div>