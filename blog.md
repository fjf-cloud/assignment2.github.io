---
layout: default
title: Blog
permalink: /blog/
---

[← Back to Home]({{ site.baseurl }}/)

## My Thoughts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
