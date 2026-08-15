# Picto legal pages

픽토 앱의 공개 약관·정책 페이지. GitHub Pages로 서비스합니다.

| 문서 | 주소 |
| --- | --- |
| 개인정보처리방침 | https://omom613.github.io/picto-legal/privacy/ |
| 이용약관 | https://omom613.github.io/picto-legal/terms/ |
| 위치기반서비스 이용약관 | https://omom613.github.io/picto-legal/location-terms/ |
| 계정 및 데이터 삭제 | https://omom613.github.io/picto-legal/account-deletion/ |

## 이 저장소의 HTML을 직접 고치지 마세요

같은 문서가 앱 안에도 있습니다. 두 벌을 손으로 맞추면 반드시 어긋납니다 —
실제로 이 방침에서 Sentry와 RevenueCat이 빠지고 계정 삭제 링크가 404가 된 적이 있습니다.

원본은 앱 저장소의 `src/constants/legal.ts` 하나입니다. 내용을 바꿀 때는 거기서 고치고,
아래를 실행해 나온 `build/legal/`을 이 저장소 루트에 덮어쓴 뒤 커밋하세요.

```bash
# picto 저장소에서
node scripts/build-legal-pages.js
```

## Play Console 설정

개인정보처리방침 URL에는 루트가 아니라 **`/picto-legal/privacy/`** 를 넣으세요.
루트(`/picto-legal/`)는 네 문서를 모아 둔 목차 페이지입니다.

Data safety 양식은 개인정보처리방침 7항(Supabase · NAVER Cloud · Sentry · RevenueCat)과
일치해야 합니다.
