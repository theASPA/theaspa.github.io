---
layout: page
title: News
permalink: /news/
---

# Testing News Page

{% raw %}{% for post in site.posts %}
- {{ post.title }} - Categories: {{ post.categories }}
{% endfor %}{% endraw %}
