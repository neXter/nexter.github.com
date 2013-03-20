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
		{% for post in site.categories.sfo-2013 %}
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