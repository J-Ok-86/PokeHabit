PokéRoutine V1.7.83 · 종료 확인 유지 / PWA 뒤로 가기 개선

반영
- 오늘 탭에서 Android 뒤로 가기: 종료하시겠습니까? → 계속 사용 / 종료
- 팝업이 열려 있으면 팝업 닫기. 다른 탭이면 오늘 탭으로 이동
- 종료 버튼에서 한 번의 클릭으로 native bridge(있는 경우), window.close(), 브라우저 이동 순으로 시도
- Android Chrome의 CloseWatcher 지원 기기에서는 가짜 방문 기록을 추가하지 않아 native Back을 방해하지 않음
- 추가 종료 안내 화면 없음
- 퀘스트·보상·기술·데이터 로직은 변경하지 않음

제약: 설치형 일반 PWA는 브라우저 보안 정책상 JavaScript에서 Android 앱을 강제로 종료하는 API가 없습니다. 따라서 기기에 따라 '종료' 버튼으로 OS Activity를 즉시 종료하는 것은 보장되지 않습니다. APK/Android WebView 래퍼의 App.exitApp 같은 네이티브 API가 있을 때는 즉시 종료가 가능합니다.

적용: JSON 백업 후 index.html, moves.html, sw.js 업로드. 설치된 PWA를 완전히 닫고 다시 실행하거나 새 버전이 설치되도록 새로고침하세요.
