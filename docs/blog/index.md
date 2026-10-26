---
layout: page
title: "动态"
permalink: /blog/
---

不定期更新的使用案例、功能说明和用户故事。没有固定的更新节奏，有想写的就写一篇。

{% for post in site.posts %}
<article style="margin: 2rem 0; padding-bottom: 1.25rem; border-bottom: 1px solid #eaeef2;">
  <h2 style="margin-bottom: 0.25rem;">
    <a href="{{ post.url | relative_url }}" style="text-decoration: none;">{{ post.title }}</a>
  </h2>
  <p style="color: #57606a; font-size: 0.9rem; margin: 0 0 0.5rem;">
    {{ post.date | date: "%Y-%m-%d" }}
    {%- if post.tags.size > 0 %} · {{ post.tags | join: " / " }}{% endif -%}
  </p>
  <p style="margin: 0;">
    {{ post.excerpt | strip_html | truncate: 160 }}
    <a href="{{ post.url | relative_url }}">阅读全文 →</a>
  </p>
</article>
{% endfor %}

{% if site.posts.size == 0 %}
<p>还没有文章，稍后再来看看。</p>
{% endif %}
