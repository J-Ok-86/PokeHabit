PokeHabit / PokeRoutine Web v1.7.138 — ChatGPT 분석용 내보내기

적용: 웹 GitHub Pages 저장소의 최상위에 ZIP 내용(index.html, moves.html, sw.js)을 덮어씁니다.
기존 데이터와 퀘스트 수동 완료, 보상 규칙, 라이프 이벤트 기능은 변경하지 않습니다.
기록 탭 > 주간 성장 브리핑 바로 아래 > 'ChatGPT 분석용 내보내기' 접이식 카드.
상단 '분석 바로가기'에서 'AI 내보내기'로 바로 이동할 수 있습니다.

기능:
- 최근 7/30/90/365일, 직접 시작일~종료일(최대 10년)을 지원합니다.
- 퀘스트, 라이프 이벤트(걷기 포함), 확정된 기상·취침, 순간생각·데일리 노트를 선택합니다.
- 개인정보 보호: 순간생각·노트는 기본 해제입니다.
- 종합 분석/개선 전략/숨은 패턴/성장 분석/직접 질문.
- 7일 이하 일별 주요 기록, 30일 이하 일별 집계, 90일 수준 주별, 긴 기간 월별 집계.
- 미리보기, 복사, 공유 버튼. 브라우저 공유 API 미지원시 복사 버튼 이용.
- 확정되지 않은 수면 추정 결과는 포함하지 않습니다.
- 예전 '하루 돌아보기'는 변함없습니다. 원본 기록은 절대 수정하지 않습니다.
- GPT 분석은 ChatGPT에서 사용자가 붙여넣거나 공유한 뒤 수행됩니다. 별도 API 키/호출 없음.
- 모바일 공유 대상 앱 목록은 Android와 각 앱의 공유 지원 여부에 따라 다릅니다.

Codespaces (웹 저장소 루트):
unzip -o PokeRoutine_v1.7.138_GPT_Analysis_Export_GitHub_Update.zip
rm -f PokeRoutine_v1.7.138_GPT_Analysis_Export_GitHub_Update.zip
git add -A
git commit -m "PokeHabit Web v1.7.138 GPT export"
git push origin main
