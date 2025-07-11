---
layout: page
title: 일상이야기
permalink: /daily/
---

🌱 개발자의 일상, 생각, 그리고 소소한 이야기들을 공유합니다.

<div class="post-list">
{% for post in site.posts %}
  {% if post.categories contains 'daily' %}
  <article class="post-preview">
    <h2>
      <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h2>
    <p class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y년 %m월 %d일" }}</time>
    </p>
    <div class="post-excerpt">
      {{ post.excerpt }}
    </div>
  </article>
  {% endif %}
{% endfor %}
</div>
