# ✂️ Cutout Studio

AI 기반 배경 제거 → Tight Crop → 3000×3000px 투명 PNG 출력까지 자동으로 처리하는 브라우저 기반 이미지 편집 도구입니다.

**[→ 바로 사용하기](https://sseung.github.io/cutout-studio/)**

## 기능

- 드래그 앤 드롭 이미지 업로드 (PNG / JPG)
- AI 배경 제거 — `@imgly/background-removal` (브라우저 내 실행, 서버 불필요)
- 불투명 픽셀 기준 Tight Crop
- 3000 × 3000px 투명 PNG 출력 (피사체 중앙 배치, 비율 유지)
- 여백(Padding) 조절 가능 (0~150px)

## 출력 스펙

| 항목 | 값 |
|------|-----|
| 크기 | 3000 × 3000px |
| 형식 | PNG (투명 배경) |
| 파일명 | `cutout_3000px.png` |

## 실행 방법

빌드 불필요 — `index.html`을 브라우저에서 바로 열거나 위 배포 링크를 사용합니다.

> 첫 실행 시 AI 모델 다운로드로 30~60초 소요될 수 있습니다. 이후 실행은 브라우저 캐시로 빠르게 동작합니다.

## 기술 스택

- HTML + CSS + Vanilla JS (빌드 없음)
- [@imgly/background-removal](https://github.com/imgly/background-removal-js) (CDN)
- Canvas API
