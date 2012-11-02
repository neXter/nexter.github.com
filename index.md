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
			<h3>My old blogs...</h3>
			<tr><td><small>2011</small></td><td> &#160; <a href="/blogs/tumblr/">Tumblr - blog.2sekunden.net</a> ({{ site.categories.tumblr | size }} Posts)</td></tr>
			<tr><td><small>2009</small></td><td> &#160; <a href="/blogs/canada/">Canada 2009</a> ({{ site.categories.canada | size }} Posts)</td></tr>
			<tr><td><small>2005-2007</small></td><td> &#160; <a href="/blogs/living-in-wow/">Living in WoW Blog</a> ({{ site.categories.living-in-wow | size }} Posts)</td></tr>
			<tr><td><small>2004-2007</small></td><td> &#160; <a href="/blogs/old-blog-v3/">2sekunden.net</a> ({{ site.categories.2sekunden | size }} Posts)</td></tr>
			<tr><td><small>2003-2004</small></td><td> &#160; <a href="/blogs/old-blog-v2/">walsweer.de - misc2go Weblog</a> ({{ site.categories.old-blog-v2 | size }} Posts)</td></tr>
			<tr><td><small>2002-2003</small></td><td> &#160; <a href="/blogs/old-blog-v1/">walsweer.de [v1]</a> ({{ site.categories.old-blog-v1 | size }} Posts)</td></tr>
		</table>
	</section>
</div>