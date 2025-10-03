---
layout: page
title: News
permalink: /news/
---

# News

{% raw %}{% for post in site.posts %}
  {% if post.categories contains "news" %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %-d, %Y" }}</p>
  {{ post.content }}
  <hr>
  {% endif %}
{% endfor %}{% endraw %}
