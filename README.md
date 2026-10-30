# PokéRoutine v0.5 — GitHub Pages 배포 안내

포켓몬 수집 방식의 개인 습관·퀘스트 기록 웹앱(PWA)입니다. 비공식 팬메이드 프로토타입입니다.

## 1. GitHub에 올리기
1. https://github.com 로그인 → New repository.
2. Repository name: `pokeroutine` / Public / Create repository.
3. 저장소 화면 → Add file → Upload files.
4. **압축파일 자체를 올리지 말고 압축 해제 후 이 폴더의 파일·하위 폴더를** 업로드하세요.
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icons/icon-192.png`
   - `icons/icon-512.png`
   - `.nojekyll`(선택)
5. Commit changes.
6. Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root) → Save.
7. 배포가 완료되면 https://<본인GitHubID>.github.io/pokeroutine/ 에 접속합니다.

## 2. 갤럭시 휴대폰/태블릿
1. Chrome에서 위 웹주소에 접속합니다.
2. 오른쪽 위 ⋮ → `앱 설치` 또는 `홈 화면에 추가` → `설치`.
3. 홈 화면에 나타난 PokéRoutine 아이콘을 눌러 실행하세요.
4. 앱 화면의 Save에서 JSON 백업, Load에서 JSON 복원 가능합니다.

## 3. 데이터 보안과 동기화
- Github Pages에 올린 앱 파일은 **누구나 볼 수 있습니다**. 이 앱에 실질적인 계정 로그인 기능은 없습니다.
- 관리자 비밀번호 1234는 소스 코드에 존재하므로 보안장치가 아닙니다.
- 퀘스트/도감/이력 데이터는 각 기기의 브라우저 저장소에 기록됩니다(자동 저장 ON 기준).
- **JSON 저장 파일은 GitHub 저장소에 업로드하지 마세요.** 개인 활동 기록이 포함되어 있습니다.
- 기기 이동: 기존 기기에서 Save → JSON 파일 전송 → 새 기기에서 Load.
- 같은 주소라도 다른 기기/브라우저는 자동 동기화되지 않습니다.
- 브라우저 데이터 삭제·앱 삭제 전에 JSON 백업을 따로 보관하세요.
- 새 HTML을 배포해도 브라우저 저장 데이터는 원칙적으로 유지되나, 도메인/경로 변경, 앱 삭제, 저장 공간 정리 등으로 손실될 수 있어 배포 전 JSON 백업을 추천합니다.

## 4. 앱 업데이트
- GitHub 저장소의 `index.html` 등 변경된 파일을 다시 업로드하고 Commit합니다.
- 기존 홈 화면 아이콘으로 다시 열면 업데이트가 반영되며, 캐시 때문에 구버전이 보이면 Chrome에서 해당 사이트를 재방문하여 새로고침합니다.
- PWA 앱 셸은 인터넷 없이도 열릴 수 있지만 포켓몬 그림은 외부 GitHub(PokeAPI)에서 가져오므로 인터넷 연결이 필요할 수 있습니다.

## 5. 공개 배포 주의
- GitHub Free에서 Pages를 쓰는 저장소는 Public이며, GitHub Pages 웹사이트는 공개됩니다.
- 포켓몬 이름·캐릭터·이미지 사용과 공개 배포에는 지식재산권 이슈가 있을 수 있습니다. 본 앱은 공식 포켓몬 서비스가 아닙니다.
