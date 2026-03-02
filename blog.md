---
layout: landing
title: Blog
description: Thoughts on AI, Jekyll, and the Modern Web.
image: assets/images/pic03.jpg
permalink: /blog/
---

# Recent Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}"><h3>{{ post.title }}</h3></a>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
    </li>
  {% endfor %}
</ul>
