---
layout: page
title: Blog
permalink: /blog/
---

# Blog

{% raw %}{% for post in site.blog %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{ post.date | date: "%B %-d, %Y" }}</p>
{{ post.content }}
<hr>
{% endfor %}{% endraw %}
