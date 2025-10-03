---
layout: page
title: News
permalink: /news/
---

# News

{% raw %}{% assign news_posts = site.posts | where: "categories", "news" %}

{% if news_posts.size > 0 %}
  {% for post in news_posts %}
  <article class="post">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
    <div class="post-content">
      {{ post.content | truncatewords: 50 }}
    </div>
    <a href="{{ post.url | relative_url }}">Read full article</a>
  </article>
  {% unless forloop.last %}<hr>{% endunless %}
  {% endfor %}
{% else %}
  <p>No news articles have been published yet.</p>
{% endif %}{% endraw %}
