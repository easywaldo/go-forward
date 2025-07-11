---
layout: home
title: Easywaldo's 블로그
---

생각과 일상을 기록하고 되새겨보는 공간입니다.

## 최근 포스트

{% for post in site.posts limit:5 %}
<article class="post-preview">
  <h2>
    <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
  </h2>
  <p class="post-meta">
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y년 %m월 %d일" }}</time>
    {% if post.categories.size > 0 %}
    • 카테고리: 
    {% for category in post.categories %}
      <span class="category">{{ category }}</span>
    {% endfor %}
    {% endif %}
  </p>
  <div class="post-excerpt">
    {{ post.excerpt }}
  </div>
</article>
{% endfor %}

## 카테고리별 포스트

<div class="category-links">
  <a href="/tech/" class="category-link">
    <h3>기술</h3>
    <p>개발 관련 포스트와 기술 학습 기록</p>
  </a>
  
  <a href="/daily/" class="category-link">
    <h3>일상이야기</h3>
    <p>개발자의 일상과 생각들</p>
  </a>
  
  <a href="/about/" class="category-link">
    <h3>내소개</h3>
    <p>블로그 운영자 소개</p>
  </a>
</div>
