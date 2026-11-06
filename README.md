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

## 로컬에서 빌드하기

필요한 도구: Git, Python 3.9 이상, Hugo extended **0.167.0** (Actions와 같은 버전)

```bash
git clone https://github.com/kotory123/kotory123.github.io.git
cd kotory123.github.io
hugo version                       # hugo v0.167.0+extended 확인
python .github/pages_build.py --build   # public/ 폴더에 사이트 생성
```

미리보기만 할 때는 `cd site` 후 `hugo server`를 실행하고 http://localhost:1313/ 을 엽니다.

## 수정하고 다시 배포하기

1. 위 표에서 고칠 파일을 수정합니다 (예: 소개 글은 `site/content/about.md`).
2. 커밋하고 `main`에 push합니다.
   ```bash
   git add -A
   git commit -m "content: 소개 글 수정"
   git push
   ```
3. 저장소 **Actions** 탭에서 `Deploy Hugo to GitHub Pages` 실행이 초록 체크인지 확인합니다.
4. https://kotory123.github.io/ 를 새로고침해 바뀐 내용을 확인합니다.

## 출처와 라이선스

- 테마: Hugo PaperMod © adityatelange, MIT License (`LICENSE`, `site/themes/template/LICENSE`)
- 배포 준비: 수업 제공 `prepare_github_pages.py` 3.1
- 글: 직접 작성. 문장 다듬기와 설정 작성에 AI(Claude)의 도움을 받았고, 내용은 직접 확인했습니다.
