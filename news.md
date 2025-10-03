---
layout: page
title: News
permalink: /news/
---

# News tp2

{% raw %}{% assign news_posts = site.posts | where: "categories", "news" %}

{% for post in news_posts %}
<article>
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <time>{{ post.date | date: "%B %-d, %Y" }}</time>
  <div>{{ post.content }}</div>
</article>
{% unless forloop.last %}<hr>{% endunless %}
{% endfor %}{% endraw %}
