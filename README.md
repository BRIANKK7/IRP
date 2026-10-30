# 로이빈 자산관리 (Roybin Family)

기존 구글 웹앱(Apps Script) 기반의 가계부 및 자산관리 도구를 **GitHub Pages**에서 사용할 수 있도록 구성한 저장소입니다.  
데이터는 기존과 동일하게 **Google Drive** 및 **Google Sheets**를 저장소로 사용합니다.

---

## 📁 파일 구조

```text
.
├── index.html     # 메인 대시보드 (카드관리, 가계부, 자산현황)
├── irp.html       # 금융투자 (IRP / ISA / 주식 / 코인 상세 현황)
├── config.js      # 구글 앱스 스크립트(GAS) 웹앱 URL 설정 파일
├── gs.txt         # 기존 구글 앱스 스크립트 백엔드 소스코드 백업
└── README.md      # 설명 문서
```

---

## 🚀 GitHub Pages 배포 방법

1. 이 저장소의 모든 파일을 GitHub 리포지토리에 푸시합니다.
2. GitHub 저장소 상단 메뉴의 **Settings**로 이동합니다.
3. 좌측 메뉴에서 **Pages**를 클릭합니다.
4. **Build and deployment** 항목의 **Branch**를 `main` (또는 `master`) 브랜치 / `/ (root)` 폴더로 설정하고 **Save**를 누릅니다.
5. 1~2분 후 생성되는 `https://<아이디>.github.io/<래포이름>/` 링크로 접속하면 모바일과 PC 브라우저에서 바로 사용하실 수 있습니다.

---

## ⚙️ 설정 (config.js)

구글 웹앱 URL이 변경될 경우 `config.js` 파일에서 `APPS_SCRIPT_URL` 주소만 변경하시면 모든 페이지에 자동 적용됩니다:

```javascript
const CONFIG = {
  APPS_SCRIPT_URL: "https://script.google.com/macros/s/.../exec"
};
```
