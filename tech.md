---
layout: posts
title: 기술
permalink: /tech/
author_profile: false
classes: wide
---

최신 기술 트렌드, 개발 경험, 그리고 배운 것들을 기록합니다.

{% assign tech_posts = site.posts | where_exp: "post", "post.categories contains 'tech'" %}
{% for post in tech_posts %}
  <article class="archive__item">
    <h2 class="archive__item-title">
      <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h2>
    <p class="archive__item-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
    <p class="page__meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y년 %m월 %d일" }}</time>
    </p>
  </article>
{% endfor %}
