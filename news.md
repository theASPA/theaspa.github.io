---
layout: page
title: News
permalink: /news/
---

# News tp3

{% raw %}{% for post in site.posts %}
  {% if post.categories contains "news" %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <time>{{ post.date | date: "%B %-d, %Y" }}</time>
    <div>{{ post.content }}</div>
  </article>
  <hr>
  {% endif %}
{% endfor %}{% endraw %}
