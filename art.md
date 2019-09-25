---
layout: page
title: Art
subtitle: Subtitle (max 140 char)
---

{% assign sorted-posts = site.posts | where: "categories","artwork" %}
{% for post in sorted-posts limit: 10 %}
<li>
<a href="{{ post.url }}">{{post.title}}</a>
</li>
{% endfor %}
