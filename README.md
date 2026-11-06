# 고영민 포트폴리오

전북대학교 초급프로젝트 과제 1 – Hugo로 만든 개인 소개 사이트입니다.

- 사이트: https://kotory123.github.io/
- 테마: [Hugo PaperMod](https://github.com/adityatelange/hugo-PaperMod) (MIT, 원본 README는 `THEME_README.md`)

## 폴더 구조

| 경로 | 역할 |
| --- | --- |
| `site/pages.json` | 사이트 설정 (제목, 언어, 메뉴, 홈 소개, GitHub 링크) |
| `site/content/about.md` | 소개 페이지 (관심 분야, 학습 목표, 사용 기술) |
| `site/content/projects/` | 활동 페이지 (캡스톤디자인 등) |
| `site/layouts/_partials/` | 테마 화면 조각을 덮어쓴 파일 (아이콘 링크 접근성) |
| `site/assets/css/extended/custom.css` | 추가 스타일 (키보드 초점, 좁은 화면 줄바꿈) |
| `site/themes/template/` | PaperMod 테마 원본 (수정하지 않음) |
| `.github/workflows/hugo-pages.yml` | GitHub Actions 빌드·배포 |
| `.github/pages_build.py` | 수업 제공 스크립트 (의존성 설치·빌드) |
