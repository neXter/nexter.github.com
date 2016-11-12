---
layout: default
title: pieter.cc
---

<div id="content">
	{% comment %}
	<section>
		<h3>Blog posts</h3>
		<table>
			{% for post in site.categories.blog %}
			<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a></td></tr>{% endfor %}
		</table>
	</section>
	{% endcomment %}
	<section>
		<h3>Traveling</h3>
		<table>
	{% comment %}
			<tr><td><small>2015</small></td><td> &#160; <a href="/blogs/usa-2015/">Trip to USA</a> ({{ site.categories.usa-2015 | size }} Posts)</td></tr>
	{% endcomment %}
			<tr><td width="80"><small>2013</small></td><td> &#160; <a href="/blogs/sfo-2013/">Trip to San Francisco</a> ({{ site.categories.sfo-2013 | size }} Posts)</td></tr>
			<tr><td><small>2009</small></td><td> &#160; <a href="/blogs/canada/">Backpacking in Canada</a> ({{ site.categories.canada | size }} Posts)</td></tr>
		</table>
	</section>
	<section>
		<h3>Old Blogs</h3>
		<table>
			<tr><td><small>2011</small></td><td> &#160; <a href="/blogs/tumblr/">Tumblr - blog.2sekunden.net</a> ({{ site.categories.tumblr | size }} Posts)</td></tr>
			<tr><td><small>2005-2007</small></td><td> &#160; <a href="/blogs/living-in-wow/">Living in WoW Blog</a> ({{ site.categories.living-in-wow | size }} Posts)</td></tr>
			<tr><td><small>2004-2007</small></td><td> &#160; <a href="/blogs/2sekunden/">2sekunden.net</a> ({{ site.categories.2sekunden | size }} Posts)</td></tr>
			<tr><td><small>2003-2004</small></td><td> &#160; <a href="/blogs/old-blog-v2/">walsweer.de - misc2go Weblog</a> ({{ site.categories.old-blog-v2 | size }} Posts)</td></tr>
			<tr><td><small>2002-2003</small></td><td> &#160; <a href="/blogs/old-blog-v1/">walsweer.de [v1]</a> ({{ site.categories.old-blog-v1 | size }} Posts)</td></tr>
		</table>
	</section>
	<section>
		<h3>Projects</h3>
		<table>
			<tr>
				<td width="80"><img class="appicon" src="/images/icon-idfa.png"></td>
				<td><strong>IDFA</strong> - A small but handy utility application to help developers and users to easily access their Apple Advertising Identifier (IDFA) for testing purposes. &raquo; <a href="https://github.com/neXter/idfa">GitHub Project</a></td>
			</tr>
		</table>
	</section>
</div>
