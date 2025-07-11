---
layout: page
title: TECH
permalink: /tech/
---

최신 기술 트렌드, 개발 경험, 그리고 배운 것들을 기록합니다.

<div class="post-list">
{% for post in site.posts %}
  {% if post.categories contains 'tech' %}
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
