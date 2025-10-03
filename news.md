---
layout: page
title: News
permalink: /news/
---

{% raw %}{% for news in site.news %}
<h2><a href="{{ news.url }}">{{ news.title }}</a></h2>
<p>{{ news.date | date: "%B %-d, %Y" }}</p>
{{ news.content }}
<hr>
{% endfor %}{% endraw %}
