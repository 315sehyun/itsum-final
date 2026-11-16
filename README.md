# 잇섬 대시보드 (Cloudflare Pages 배포용)

`index.html` 한 파일이 대시보드 전체입니다. 스크립트·데이터·로고가 모두 들어 있어 다른 파일이 필요 없습니다. 외부 연결은 Google Fonts뿐입니다.

- 원본: `itsum-v3/dist/itsum.html` (2026-11-16 빌드, D66, 테스트 183/183)
- 기준 시각: 2026-11-18 15:00 고정 (`config.demoNow`)
- 화면 상태는 브라우저 localStorage에 저장됩니다(방문자마다 따로).

## Cloudflare Pages 설정

| 항목 | 값 |
|---|---|
| Framework preset | None |
| Build command | (비움) |
| Build output directory | `/` (이 파일들이 저장소 맨 위에 있을 때). 하위 폴더에 두었다면 그 폴더 이름 |

대시보드를 고친 뒤에는 `itsum-v3`에서 `tools/build-artifact.ps1`로 다시 빌드하고, `dist/itsum.html`을 이 폴더의 `index.html`로 덮어써서 올립니다.
