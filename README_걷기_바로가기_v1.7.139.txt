PokeHabit / PokeRoutine 웹 업데이트 v1.7.139 — 걷기 통계 바로가기

변경 내용:
1. 기록 탭 맨 위 분석 바로가기 안에 [🚶 걷기 통계] 버튼 추가.
2. 설정 > 라이프 이벤트 > 걷기 통계 표시가 ON일 때만 바로가기를 표시함 (기본 OFF 그대로 유지).
3. 클릭 시 기존 걷기 통계 섹션으로 이동. 섹션은 ON인 경우 이미 펼쳐진 상태임.
4. 모바일(699px 이하)에서는 3열 배치, 더 넓은 화면에서는 최대 6열 배치.
5. 기존 걷기 통계 계산/기록/보상/퀘스트/APK 연동에는 변경 없음.

적용: 기존 GitHub Pages PokeHabit 웹 저장소 루트에 이 ZIP을 업로드하여 덮어쓰기.
APK Wrapper는 GitHub Pages의 웹 화면을 읽으므로 Android 소스 업데이트/재빌드는 필요 없음.
웹 캐시 버전 갱신 포함. 설치된 PWA에서 이전 내용이 보이면 새로고침 또는 재실행.

Codespaces 웹 저장소 루트 Bash:
unzip -o PokeRoutine_v1.7.139_Walk_Statistics_Shortcut_GitHub_Update.zip
rm -f PokeRoutine_v1.7.139_Walk_Statistics_Shortcut_GitHub_Update.zip
git add -A
git commit -m "PokeHabit Web v1.7.139 walk stats shortcut"
git push origin main
