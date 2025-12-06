---
title: Blog
icon: fas fa-blog
order: 1
layout: page
---

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }})  
  <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
{% endfor %}