# GitHub Copilot Instructions

이 프로젝트는 Jekyll 기반의 개발자 블로그입니다.

## 프로젝트 구조

- `_posts/`: 블로그 포스트 (마크다운 파일)
- `_layouts/`: 페이지 레이아웃 템플릿
- `_sass/`: Sass 스타일시트 파일
- `tech.md`, `daily.md`, `about.md`: 카테고리 페이지

## 포스트 작성 가이드

새로운 포스트를 작성할 때는 다음 형식을 사용하세요:

```markdown
---
layout: post
title: "포스트 제목"
date: YYYY-MM-DD HH:MM:SS +0900
categories: [tech] # 또는 [daily]
tags: [태그1, 태그2]
excerpt: "포스트 요약"
---

# 포스트 내용
```

## 카테고리

- `tech`: 기술 관련 포스트
- `daily`: 일상 이야기

## 댓글 기능

Disqus 댓글 시스템을 사용합니다. `_config.yml`에서 `disqus.shortname`을 설정하세요.

## 로컬 개발

```bash
bundle install
bundle exec jekyll serve
```

## GitHub Pages 배포

이 블로그는 GitHub Pages에 배포할 수 있습니다. 저장소 설정에서 Pages를 활성화하세요.
