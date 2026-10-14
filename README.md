# 90일 울산 · 부울경 청년 창업부트캠프 2기 랜딩 (90ulsan.kr)

GitHub Pages 배포용 최종 파일 (2026-10-14, v18)

## 폴더 구조
- `index.html` — 모바일(앱) 랜딩. 화면 폭 1024px 이상이면 자동으로 `pc/`로 이동
- `pc/index.html` — 웹(PC) 랜딩. 좁은 화면에서 열면 다시 모바일로 이동
- `assets/` — 이미지·폰트·아이콘 (두 페이지가 같이 씀)
- `CNAME` — 도메인 90ulsan.kr
- `.nojekyll` — GitHub Pages가 파일을 그대로 쓰게 하는 빈 파일 (지우지 말 것)
- `favicon.ico`, `robots.txt`, `sitemap.xml`

강제 보기: 모바일판 `90ulsan.kr/?m=1`, PC판 `90ulsan.kr/pc/?pc=1`

## 배포 순서
1. GitHub 새 public 저장소 만들기 → 이 폴더 안의 파일 전부를 저장소 맨 위(root)에 업로드
   (폴더째가 아니라 안의 내용물을 올려야 함. `.nojekyll`처럼 점으로 시작하는 파일도 꼭 포함)
2. Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save
3. Custom domain에 `90ulsan.kr` 확인 (CNAME 파일로 자동 입력됨)
4. 도메인 DNS(카페24)
   - A 레코드 4개: 185.199.108.153 / 185.199.109.153 / 185.199.110.153 / 185.199.111.153
   - www CNAME → `<깃허브아이디>.github.io`
5. DNS 반영 후 Pages 화면에서 Enforce HTTPS 체크
6. 휴대폰·PC로 90ulsan.kr 접속 확인, 포스터 QR 실기 확인

## 연결된 링크 (config 기준)
- 사전 신청: Typeform `https://form.typeform.com/to/xKP8suXq`
- 커뮤니티 밋업 신청: Google Form (울산 스타트업 커뮤니티 밋업 신청)
- Meta 픽셀 ID: 아직 비어 있음 → 받으면 빌드에 넣어 다시 배포
