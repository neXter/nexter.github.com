---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>Canada 2009</h2>
		Backpacking for four weeks
	</section>
	<section>
		{% for post in site.categories.canada %}
		    {% unless post.next %}
      			{{ post.date | date_to_long_string }}<br/>
    		{% else %}
    		  {% capture day %}{{ post.date | date: '%D' }}{% endcapture %}
    		  {% capture nday %}{{ post.next.date | date: '%D' }}{% endcapture %}
    		  {% if day != nday %}
				<br/>{{ post.date | date_to_long_string }}<br/>
    		  {% endif %}
    		{% endunless %}
		<a href="{{ post.url }}">{{ post.title }}</a><br/>
		{% endfor %}
	</section>
</div>