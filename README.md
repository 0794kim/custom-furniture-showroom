# Developer Portfolio

HTML, CSS, JavaScript로 제작한 반응형 개발자 포트폴리오입니다. 별도의 빌드 도구나 프레임워크 없이 GitHub Pages에서 동작합니다.

## 주요 기능

- 데스크톱·태블릿·모바일 반응형 레이아웃
- 프로젝트 사례 중심의 단일 페이지 구성
- 모바일 내비게이션
- 스크롤 등장 애니메이션
- 키보드 탐색과 모션 감소 설정
- GitHub Actions 자동 배포

## 프로젝트 구조

```text
.
├── .github/
│   └── workflows/
│       └── pages.yml
├── index.html
├── styles.css
├── script.js
└── README.md
```

## 로컬에서 실행

`index.html`을 직접 열거나 정적 서버를 실행합니다.

```powershell
python -m http.server 8000
```

실행 후 `http://localhost:8000`으로 접속합니다.

## GitHub Pages 자동 배포

`main` 브랜치에 변경사항을 push하면 `.github/workflows/pages.yml`이 사이트 파일을 업로드하고 GitHub Pages에 자동 배포합니다. GitHub 저장소의 **Settings → Pages → Build and deployment → Source**가 **GitHub Actions**로 설정되어 있어야 합니다.

수동 배포가 필요하면 저장소의 **Actions → Deploy static site to GitHub Pages → Run workflow**를 사용합니다.

## 콘텐츠 수정

- `index.html`: 이름, 소개, 프로젝트, 이메일 및 외부 링크
- `styles.css`: 색상, 타이포그래피, 간격 및 반응형 레이아웃
- `script.js`: 모바일 메뉴와 스크롤 애니메이션

## 기술 스택

- HTML5
- CSS3
- Vanilla JavaScript
- GitHub Actions
- GitHub Pages
