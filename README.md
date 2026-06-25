# 🚔 경찰급여 계산기 — 배포 가이드

## 파일 구성
```
police-salary-app/
├── index.html     ← 앱 본체
├── manifest.json  ← PWA 설정
├── sw.js          ← 오프라인 캐시
└── icons/         ← 앱 아이콘 폴더 (직접 추가 필요)
    ├── icon-192.png
    └── icon-512.png
```

## 1. Vercel로 배포 (무료, 추천)

1. https://vercel.com 가입 (GitHub 계정으로 로그인)
2. "Add New Project" → "Browse" → 이 폴더 업로드
3. 배포 완료! → yourapp.vercel.app 주소 생성

## 2. 아이콘 만들기
- https://realfavicongenerator.net 접속
- 원하는 이미지 업로드 → 192x192, 512x512 PNG 다운로드
- icons/ 폴더에 저장

## 3. 스마트폰에서 앱처럼 사용하기 (PWA)
- Safari(iOS): 공유 버튼 → "홈 화면에 추가"
- Chrome(Android): 주소창 옆 설치 버튼 or 메뉴 → "앱 설치"

## 4. 광고 붙이기 (AdSense)
1. https://adsense.google.com 신청
2. 심사 통과 후 index.html <head>에 아래 코드 추가:
```html
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXX" crossorigin="anonymous"></script>
```
3. 광고 단위 생성 후 원하는 위치에 삽입

## 5. 카카오 애드핏 (한국 사용자 특화)
- https://adfit.kakao.com 신청
- AdSense보다 심사 빠름, 모바일 광고 단가 좋음
