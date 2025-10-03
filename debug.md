---
layout: page  
title: Debug
permalink: /debug/
---

**Total Posts:** {{ site.posts | size }}

**Posts with 'news' category:**
{% for post in site.posts %}
  {% if post.categories contains "news" %}
  - "{{ post.title }}" 
  {% endif %}
{% endfor %}

**Raw categories dump:**
{% for post in site.posts %}
- {{ post.title }}: [{{ post.categories | join: ", " }}]
{% endfor %}
