PokéRoutine V1.7.84 · 종료 버튼의 브라우저 뒤로 가기 경로 보완

변경 사항
- 뒤로 가기: 팝업 닫기 → 다른 탭에서 오늘 탭 → 오늘 탭에서 종료 확인
- 종료 선택 시 추가 화면을 띄우지 않고 현재 이벤트에서 browser history back을 호출
- 기존 CloseWatcher를 해제해 종료 확인으로 되돌아가는 루프 제거
- 브라우저가 허용하는 경우 history.go(-2), history.back 또는 window.close 시도
- 백업 데이터/보상/퀘스트 로직 유지

주의: Chrome 등의 일반 설치형 PWA에서는 자바스크립트로 Android 하드웨어 Back을 합성하거나 앱 Activity를 확실히 종료하는 표준 API가 없습니다. 따라서 버튼 한 번으로 실제 OS 차원의 강제 종료까지 보장할 수 없습니다. 지원 가능한 네이티브 래퍼에서는 App.exitApp 경로를 우선 사용합니다.

설치: 기존 JSON 데이터 백업 후 index.html, moves.html, sw.js를 GitHub에 덮어쓴 뒤 설치된 앱을 재실행하세요.
