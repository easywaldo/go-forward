---
layout: posts
title: 일상이야기
permalink: /daily/
author_profile: false
classes: wide
---

개발자의 일상, 생각, 그리고 소소한 이야기들을 공유합니다.

{% assign daily_posts = site.posts | where_exp: "post", "post.categories contains 'daily'" %}
{% for post in daily_posts %}
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
