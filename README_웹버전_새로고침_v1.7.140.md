# PokeHabit Web v1.7.140

## 추가 기능
- APK의 지원 여부(`webRefreshSupported`)를 확인한 다음에만 `설정 → 앱 관리` 메뉴를 표시.
- 해당 메뉴의 버튼을 누르면 Android Wrapper에 새로고침 요청.
- 서버 확인에 실패하면 현재 페이지·로컬 데이터·캐시 유지.
- PWA 및 이전 APK에는 메뉴가 나타나지 않으며 기존 기능과 동작을 유지.
- `sw.js`의 앱 쉘 캐시 버전 변경: 새로운 앱 파일이 설치될 때 기존 앱 쉘 캐시 정리.

## GitHub Codespaces (Bash)

```bash
unzip -o PokeRoutine_v1.7.140_Safe_Web_Refresh_GitHub_Update.zip
rm -f PokeRoutine_v1.7.140_Safe_Web_Refresh_GitHub_Update.zip
git add -A
git commit -m "PokeHabit Web v1.7.140 refresh settings"
git push origin main
```

**배포 순서**: 웹 v1.7.140 → Android v1.0.14.
새로고침 버튼은 최신 Android Wrapper로 업데이트한 뒤에만 나타납니다.
