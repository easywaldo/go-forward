# Enjoy challenge and go foward 🚀

Jekyll 기반의 개발자 블로그입니다. 기술과 일상을 기록하고 공유합니다.

## 🎯 특징

- **Jekyll 정적 사이트 생성기** 사용
- **마크다운 기반** 포스트 작성
- **카테고리별 분류**: 기술, 일상이야기, 내소개
- **댓글 기능**: Disqus 통합
- **반응형 디자인**: 모바일 최적화
- **GitHub Pages** 자동 배포

## 📁 프로젝트 구조

```
├── _config.yml          # Jekyll 설정 파일
├── _posts/              # 블로그 포스트 (마크다운)
├── _layouts/            # 페이지 레이아웃 템플릿
├── _sass/               # Sass 스타일시트
├── assets/              # CSS, JS, 이미지 등
├── tech.md              # 기술 카테고리 페이지
├── daily.md             # 일상이야기 카테고리 페이지
├── about.md             # 내소개 페이지
├── index.md             # 메인 페이지
└── .github/
    └── workflows/       # GitHub Actions 워크플로우
```

## 🛠️ 로컬 개발

### 1. 저장소 클론

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
```

### 2. 의존성 설치

```bash
bundle install
```

### 3. 로컬 서버 실행

```bash
bundle exec jekyll serve
```

브라우저에서 `http://localhost:4000`으로 접속하여 확인할 수 있습니다.

## 📝 포스트 작성하기

### 1. 새 포스트 파일 생성

`_posts/` 디렉토리에 `YYYY-MM-DD-title.md` 형식으로 파일을 생성합니다.

### 2. Front Matter 설정

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

마크다운 형식으로 내용을 작성합니다.
```

### 3. 카테고리 분류

- `tech`: 기술 관련 포스트
- `daily`: 일상 이야기

## 💬 댓글 기능 설정

1. [Disqus](https://disqus.com/)에서 계정을 생성하고 사이트를 등록합니다.
2. `_config.yml` 파일에서 `disqus.shortname`을 설정합니다:

```yaml
disqus:
  shortname: your-disqus-shortname
```

## 🌐 GitHub Pages 배포

### 1. GitHub 저장소 설정

1. GitHub에서 새 저장소를 생성합니다.
2. 저장소 이름을 `username.github.io` 형식으로 설정합니다.

### 2. Pages 설정

1. 저장소 Settings > Pages 메뉴로 이동합니다.
2. Source를 "GitHub Actions"로 설정합니다.
3. 코드를 push하면 자동으로 빌드 및 배포됩니다.

### 3. 사이트 URL

배포가 완료되면 `https://username.github.io`에서 블로그를 확인할 수 있습니다.

## 🎨 커스터마이징

### 사이트 정보 수정

`_config.yml` 파일에서 다음 항목들을 수정하세요:

```yaml
title: easywaldo 의 이야기
email: your-email@example.com
description: 기술과 일상을 기록하는 개발자의 블로그입니다.
github_username: your-github-username
```

### 스타일 수정

`_sass/custom.scss` 파일에서 CSS 스타일을 커스터마이징할 수 있습니다.

## 🔧 기술 스택

- **Jekyll**: 정적 사이트 생성기
- **Minima**: Jekyll 테마
- **Sass**: CSS 전처리기
- **Disqus**: 댓글 시스템
- **GitHub Pages**: 호스팅
- **GitHub Actions**: 자동 배포

## 📄 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다.

## 🤝 기여하기

이슈 제기와 PR을 환영합니다!

---

*Happy blogging! 🎉*
