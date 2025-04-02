---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog-archive">
  <h1 class="page-title">Blog Yazıları</h1>
  
  <div class="posts-list">
    {% for post in site.posts %}
      <div class="post-card">
        <div class="post-meta">
          <span class="post-date">{{ post.date | date: "%d %b %Y" }}</span>
          {% if post.categories.size > 0 %}
            <span class="post-categories">
              {% for category in post.categories %}
                <a href="/categories/{{ category | slugify }}">{{ category }}</a>
              {% endfor %}
            </span>
          {% endif %}
        </div>
        <h3 class="post-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <div class="post-excerpt">
          {{ post.excerpt | strip_html | truncatewords: 30 }}
        </div>
        <a href="{{ post.url | relative_url }}" class="read-more">Devamını Oku →</a>
      </div>
    {% endfor %}
  </div>
</div>