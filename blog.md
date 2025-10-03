---
layout: page
title: Blog
permalink: /blog/
---


testing lq 


{% raw %}{% for post in site.blog %}
<h2>{{ post.title }}</h2>
<p>{{ post.date | date: "%B %-d, %Y" }}</p>
{{ post.content }}
<hr>
{% endfor %}{% endraw %}
