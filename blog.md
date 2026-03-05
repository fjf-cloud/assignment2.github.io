---
layout: default
title: Blog
permalink: /blog/
---

[← Back to Home]({{ site.baseurl }}/)

## My Thoughts

<div class="blog-feed">
  {% for post in site.posts %}
    <article style="margin-bottom: 50px; border-bottom: 2px solid #e1e4e8; padding-bottom: 30px;">
      <h2 style="color: #1e3a5f; margin-bottom: 10px;">
        <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">{{ post.title }}</a>
      </h2>
      
      <p style="color: #6a737d; font-size: 0.9rem; font-style: italic;">
        Published on {{ post.date | date: "%B %d, %Y" }}
      </p>

      <div class="post-content" style="line-height: 1.6;">
        {{ post.content }}
      </div>
    </article>
  {% endfor %}
</div>
