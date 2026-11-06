---
title: "개인 포트폴리오 사이트 제작 (초급프로젝트 과제)"
date: 2026-11-06
summary: "Hugo PaperMod 테마와 GitHub Actions로 이 사이트를 만들고 자동 배포한 과정. 개인 작업."
---

## 한눈에 보기 {#overview}

| 항목 | 내용 |
| --- | --- |
| 기간 | 2026년 11월 |
| 상태 | 완료 (내용은 계속 추가) |
| 형태 | 개인 작업 (초급프로젝트 과제 1) |
| 저장소 | [kotory123/kotory123.github.io](https://github.com/kotory123/kotory123.github.io) |

**목적:** 내 소개와 활동을 한곳에 모으고, main에 push하면 자동으로 빌드·배포되는 흐름을 직접 만들어 보는 것입니다.

## 수행 과정 {#process}

1. **테마 선택:** 문서·블로그형이면서 메뉴·모바일 화면이 기본으로 갖춰진 PaperMod를 골랐습니다. 소개 글과 활동 글을 나눠 쓰기 쉽고, 별도 Node 빌드 없이 Hugo만으로 빌드됩니다.
2. **배포 준비:** 테마 ZIP을 풀고 수업 제공 스크립트로 GitHub Actions 워크플로를 만든 뒤, Settings → Pages에서 Source를 GitHub Actions로 정했습니다.
3. **내용 작성:** 설정(`site/pages.json`)과 글(`site/content/`)을 작은 단위로 나눠 커밋했습니다.
4. **점검과 수정:** 1440px·768px·390px 화면, 키보드(Tab) 이동, 링크와 404 요청을 확인하고 고쳤습니다.
