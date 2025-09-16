---
layout: default
title: Blog
permalink: /blog
---

# Blog

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | prepend: site.baseurl }}) — {{ post.date | date: "%b %d, %Y" }}
{% else %}
_No posts yet._
{% endfor %}

[Back Home]({{ site.baseurl }}/)
