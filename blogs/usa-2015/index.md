---
layout: default
title: pieter.cc
---

<div id="content">

	<section>
		<h2>USA 2013</h2>
		07.08. bis 11.09.2015, erst 2 Wochen Arbeit, dann 3 Wochen Urlaub.
	</section>
	<section>
		{% for post in site.categories.usa-2015 %}
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