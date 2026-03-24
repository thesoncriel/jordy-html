# 죠르디 (JORDY) 소개 웹페이지

카카오프렌즈 니니즈의 사랑스러운 민트 공룡, **죠르디**를 소개하는 웹페이지입니다.

> 이 프로젝트는 **Vibe Coding**으로 만들어졌습니다.
> 사람이 직접 코드를 작성한 것이 아니라, AI(Claude Code)와 자연어로 대화하며 기획부터 배포까지 진행했습니다.

## 배포 URL

https://thesoncriel.github.io/jordy-html/

## 기술 스택

- HTML
- Tailwind CSS (CDN)
- GitHub Actions + GitHub Pages

## 프로젝트 히스토리

이 프로젝트는 아래와 같은 과정으로 만들어졌습니다.

### 1단계: 기본 HTML 페이지 생성

- "죠르디 소개 웹페이지를 만들어줘"라는 요청으로 시작
- Claude Code가 인터넷에서 죠르디 캐릭터 정보를 검색하여 수집
- 프로필, 소개, 재미있는 사실, 갤러리 섹션을 포함한 HTML 페이지를 생성
- 카카오 공식 CDN에서 죠르디 이미지를 찾아 적용

### 2단계: Tailwind CSS 전환

- 기존 인라인 CSS(`<style>` 태그)를 Tailwind CSS 유틸리티 클래스로 전환
- Tailwind CDN을 사용하여 별도 빌드 과정 없이 적용
- 죠르디 테마에 맞는 커스텀 컬러(`jordy`) 정의

### 3단계: 이미지 로컬화

- 외부 CDN 이미지 URL을 로컬 `images/` 폴더로 다운로드
- HTML 경로를 로컬 상대 경로(`./images/`)로 변경
- 오프라인에서도 정상 표시 가능하도록 개선

### 4단계: GitHub 배포

- GitHub CLI(`gh`)를 설정하고 인증
- `jordy-html` public 리포지토리 생성 및 push
- GitHub Actions 워크플로우를 추가하여 GitHub Pages 자동 배포 구성

### 5단계: 콘텐츠 개선 (PR)

- "쬬르디" 텍스트에 카카오 공식 소개 페이지 하이퍼링크 추가
- 직접 push가 아닌 Pull Request 방식으로 코드 리뷰 프로세스 적용

## 폴더 구조

```
jordy-html/
├── index.html
├── images/
│   ├── jordy-kv.png
│   ├── jordy.png
│   ├── jordy-1.png
│   └── jordy-2.png
├── .github/
│   └── workflows/
│       └── deploy.yml
└── README.md
```

## 관련 링크

- [죠르디 인형 구매 (다나와)](https://search.danawa.com/dsearch.php?query=%EC%A3%A0%EB%A5%B4%EB%94%94+%EC%9D%B8%ED%98%95)

## 저작권

죠르디 캐릭터 및 이미지의 저작권은 [카카오](https://www.kakaocorp.com)에 있습니다.

---

🤖 Generated with [Claude Code](https://claude.com/claude-code)
