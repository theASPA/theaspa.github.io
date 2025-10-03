---
layout: page
title: News
permalink: /news/
---

# ASPA News

The latest updates, achievements, and official reports from our organization.

---

{% raw %}{% for post in site.categories.news %}
<div class="news-item">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-meta">Published on {{ post.date | date: "%B %-d, %Y" }}</p>
  {{ post.excerpt }}
  <p><a href="{{ post.url }}">Read more →</a></p>
</div>
<hr>
{% endfor %}{% endraw %}
