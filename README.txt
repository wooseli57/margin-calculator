최대비용 마진계산기 PWA 배포 파일

[구성]
index.html            앱 본체
manifest.webmanifest  앱 이름·아이콘·색 (설치용 정보)
sw.js                 오프라인 사용을 위한 서비스 워커
icons/                앱 아이콘 (192, 512, 마스커블, 아이폰용)

[GitHub Pages로 배포]
1. github.com 로그인 → 오른쪽 위 + → New repository
   이름: margin-calculator, Public 선택 → Create repository
2. "uploading an existing file" 클릭 → 압축을 푼 파일 전부(icons 폴더 포함)를 끌어다 놓기 → Commit changes
3. 저장소 Settings → Pages → Source: Deploy from a branch → Branch: main, /(root) → Save
4. 1~2분 뒤 https://(깃허브 아이디).github.io/margin-calculator/ 로 접속

[폰에 설치]
- 안드로이드(크롬): 앱 위쪽 "설치" 버튼 또는 메뉴 → 홈 화면에 추가
- 아이폰(사파리): 아래쪽 공유 버튼 → 홈 화면에 추가
- PC(크롬·엣지): 주소창 오른쪽 설치 아이콘

[수정할 때]
index.html을 고친 뒤 sw.js 맨 위 VERSION 숫자를 올려서(margin-v1 → margin-v2) 함께 올리면
사용자 기기에도 새 버전이 반영됩니다.
