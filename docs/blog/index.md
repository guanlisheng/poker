---
layout: page
title: 产品动态
description: 西瓜大屏的使用指南、功能说明和产品动态。
permalink: /blog/
---

# 产品动态

这里整理西瓜大屏的使用指南、功能说明和场景案例，帮助你在正式部署前了解产品。

{% assign posts = site.posts | sort: "date" | reverse %}

{% for post in posts %}
<article class="blog-entry">
  <h2>
    <a href="{{ post.url | relative_url }}">
      {{ post.title | escape }}
    </a>
  </h2>

  <p class="post-meta">
    <time datetime="{{ post.date | date_to_xmlschema }}">
      {{ post.date | date: "%Y-%m-%d" }}
    </time>

    {% for tag in post.tags %}
      <span class="tag">{{ tag | escape }}</span>
    {% endfor %}
  </p>

  {% if post.description %}
    <p>{{ post.description | escape }}</p>
  {% else %}
    <p>{{ post.excerpt | strip_html | normalize_whitespace | truncate: 180 }}</p>
  {% endif %}

  <p>
    <a href="{{ post.url | relative_url }}">阅读全文 →</a>
  </p>
</article>
{% endfor %}

{% if posts.size == 0 %}
目前还没有文章。请稍后再来查看。
{% endif %}
