# CHANGELOG

## 2026-06-17
### Fixed / Improved
- 스크롤 잰크 완화: 상단 nav의 `backdrop-filter: blur` 제거(모바일 버벅임 주원인), 스크롤 핸들러 requestAnimationFrame 스로틀 + passive.
- 히어로 `height: 100svh` 폴백 추가(모바일 인앱 웹뷰의 100vh 계산 오류 대응).
- 모바일(≤960px)에서는 스크롤 페이드 애니메이션 비활성화 → 스크롤이 부드럽고, 인앱 웹뷰에서 IntersectionObserver가 불안정해도 콘텐츠가 항상 보이게(흰화면 방지). 데스크탑은 기존 페이드 유지.
- 히어로는 중앙 정렬 유지, 모바일 하단 바는 추가하지 않음(기존 '체험 예약' 플로팅 버튼 유지).
