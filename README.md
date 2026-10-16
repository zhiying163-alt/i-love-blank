# I ♥ ___

밀턴 글레이저의 I ♥ NY(1977)를 웹 경험으로 리디자인한 작업.
원작의 리버스 구조(단어·기호·약자)에서 출발해, 하트 다음의 빈칸을 보는 사람이 직접 채우도록 했다.

- 디자인과 생활 · 디자이너 연구 리디자인 과제
- 사이트: `https://<GitHub 아이디>.github.io/<저장소 이름>/`

## 구성

| 섹션 | 내용 |
| --- | --- |
| 1977 | 원작 로고와 리퀴드 글래스 하트 렌즈 |
| Explore | 뉴욕 다섯 장면. 하트 렌즈로 에칭 위에 색을 드러낸다 |
| Make | 빈칸에 단어를 넣어 나만의 I ♥ ___ 포스터를 만들고 PNG로 저장 |
| Wall | 만든 포스터를 모아 보는 벽 (브라우저에만 저장) |

## 파일 구조

```
index.html
assets/
  fonts/   Instrument Serif, Courier Prime, Cutive, Pretendard (woff2)
  img/     장면별 에칭·컬러 이미지(webp), 파비콘
.nojekyll
```

## 로컬에서 열기

PNG 저장과 WebGL 효과는 `file://`로 열면 브라우저 보안 정책 때문에 동작하지 않을 수 있다. 로컬 서버로 연다.

```
python3 -m http.server 8000
# http://localhost:8000
```

## 사용 기술

- HTML, CSS, JavaScript (빌드 도구 없음)
- WebGL: 원작 하트 형태로 만든 높이맵 기반 굴절 렌즈
- [GSAP](https://gsap.com) 3.12 + ScrollTrigger, [Lenis](https://lenis.darkroom.engineering) 1.1 (index.html에 포함)

## 폰트

- Instrument Serif, Courier Prime: SIL Open Font License 1.1
- Pretendard: SIL Open Font License 1.1
- Cutive: SIL Open Font License 1.1 (사용자가 채우는 단어)
- 포스터의 I와 NY는 1977년 원작 로고의 글자 형태를 그대로 그린다.

## 고지

I ♥ NY 로고는 뉴욕주 경제개발부(Empire State Development)의 등록 상표다. 이 저장소는 수업 과제용 비상업 작업이며, 원작 로고와 사진의 권리는 각 권리자에게 있다.
