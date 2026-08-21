# ANITRIP — 송유진 UI/UX 포트폴리오

## 파일
- `index.html` — 사이트 본체 (Tailwind는 이미 CSS로 컴파일되어 내장, CDN 경고 없음)
- `assets/` — 앱 화면 13장 + MVP + 린캔버스 + 로고
- `fonts/` — Paperlogy 서브셋 (400/500/600/700, woff2)

## 폰트
- 본문: Paperlogy (업로드한 TTF를 페이지에 쓰인 글자만 남겨 woff2로 서브셋 — 파일당 28KB)
- 헤드라인: JalnanGothic (jsDelivr 웹폰트 링크)
  `https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_231029@1.1/JalnanGothic.woff`
  오프라인에서도 쓰려면 JalnanGothic.woff를 `fonts/`에 넣고 index.html의 @font-face src를 바꾸세요.

## 배포
GitHub Pages / Netlify / Vercel에 이 폴더 그대로 올리면 됩니다.

## Tailwind 재빌드가 필요할 때
클래스를 새로 추가했다면:
```
npm i -D tailwindcss@3
npx tailwindcss -c tailwind.config.js -i in.css -o out.css --minify
```
로 만든 CSS를 index.html의 첫 번째 <style> 안에 교체하세요.
