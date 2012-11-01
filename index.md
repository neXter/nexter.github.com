---
layout: default
title: pieter.cc
---

<div id="content">
	<section>
		<h3>Blog posts</h3>
			<table>
    		{% for post in site.posts %}
      		<tr><td><small>{{ post.date | date_to_long_string }}</small></td><td> &#160; <a href="{{ post.url }}">{{ post.title }}</a><br/></td></tr>
    		{% endfor %}
    		</table>
	</section>
</div>

{% comment %}
    	{% for post in paginator.posts %}
		<section>
			<div class="post contain">
				<time>{{ page.date | date_to_long_string }}</time>
				<h1><a href="{{ page.url }}">{{ page.title }}</a></h1>

				{{ content }}
			</div>
		</section>
	{% endfor %}
</div>

<nav class="pagination">
  {% if paginator.previous_page %}
    <span class="previous">
		<a href="/page{{paginator.previous_page}}" rel="previous">&lt; Previous</a>
	</span>
  {% else %}
    <span class="previous">Previous</span>
  {% endif %}
  <span class="page_number ">Page: {{paginator.page}} of {{paginator.total_pages}}</span>
  {% if paginator.next_page %}
    <span class="next">
	    <a href="/page{{paginator.next_page}}" rel="next" >Next &gt;</a>
	</span>
  {% else %}
    <span class="next ">Next</span>
  {% endif %}
</nav>
{% endcomment %}