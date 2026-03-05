
---
layout: default
title: Blog
permalink: /blog/
---

[← Back to Home]({{ site.baseurl }}/)

<div class="blog-feed">
  {% for post in site.posts %}
    <article style="margin-bottom: 60px; border-bottom: 2px solid #f0f0f0; padding-bottom: 40px;">
      <header>
        <h2 style="margin-bottom: 5px; color: #1e3a5f;">
          <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">{{ post.title }}</a>
        </h2>
        <p style="color: #888; font-size: 0.9rem; font-style: italic;">
          Published on {{ post.date | date: "%B %d, %Y" }}
        </p>
      </header>

      <div class="post-entry" style="line-height: 1.8; color: #333;">
        {{ post.content }}
      </div>
    </article>
  {% endfor %}
</div>
