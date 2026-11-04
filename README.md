# ttl-proposal.github.io

더테니스럭스 아카데미 코치님을 위한 웹 프로젝트 제안서입니다.

- 공개 주소: https://the-tennis-lux.github.io/ttl-proposal.github.io/
- 구성: 개요 · 화면 구성 · 제공 기능 · 운영비 컨설팅 · 코치님 결정사항
- `index.html`: 외부 실행 파일 없이 동작하는 탭형 제안서
- `.nojekyll`: 정적 파일을 그대로 배포하도록 지정

## 확인할 점

회원 승인 화면과 계산기는 설명용 예시입니다. 실제 회원 데이터, 상담 접수, 로그인, 결제 기능은 연결되어 있지 않습니다. 예시 이메일은 `example.com` 주소입니다. 금액은 제안서의 가정에 따른 예상치이며 실제 청구액이나 확정 견적이 아닙니다.

## 게시 및 수정

GitHub 저장소의 Settings → Pages에서 `Deploy from a branch`, `main`, `/ (root)`를 선택합니다. `main`에 변경을 push하면 GitHub Pages가 다시 배포합니다. 별도 빌드나 패키지 설치가 필요하지 않습니다.

이 저장소는 조직 대표 사이트 이름과 다르므로 프로젝트 경로 `/ttl-proposal.github.io/`를 사용합니다. 사용자 지정 도메인은 설정하지 않습니다.

## 검증 및 복구

수정 후 HTML의 목차 링크, 작은 화면 배치, 회원 승인 예시, 월 비용 계산기를 확인합니다. 공개해도 되는 자료만 넣고 실제 회원 연락처·사진·인증 정보를 추가하지 않습니다.

배포 오류가 생기면 Actions의 Pages 배포 결과를 확인합니다. 이전 상태로 되돌릴 때는 해당 변경을 `git revert`로 되돌린 후 push합니다. 기존 커밋 기록을 강제로 덮어쓰지 않습니다.

## 화면별 탐색

상단 탭을 선택하면 해당 화면만 표시됩니다. `#overview`, `#layout`, `#features`, `#budget`, `#decisions`로 직접 열 수 있고 세부 항목 링크와 브라우저 뒤로/앞으로 이동도 지원합니다. 키보드는 좌우 방향키·Home·End로 탭을 이동하고 Enter 또는 Space로 선택합니다. Tab 키로 선택한 화면에 진입할 수 있습니다.

탭을 바꿔도 계산기 입력과 회원 승인 예시 상태를 유지합니다. 새로고침하면 예시 상태는 초기화됩니다. 인쇄/PDF에는 전체 내용을 표시하며 JavaScript가 꺼져 있으면 기존 문서처럼 전체를 읽을 수 있습니다.

### 제공 기능의 상세 탭

제공 기능 화면 안에 랜딩·상담·회원가입/코치 승인·공개 갤러리·일정 탭이 있습니다. 각각 `#feature-landing`, `#feature-consultation`, `#feature-membership`, `#feature-gallery`, `#feature-schedule` 주소로 바로 열 수 있습니다. 기존 `#coach`, `#consultation`, `#gallery-policy` 링크도 해당 상세 탭을 자동으로 엽니다. 상세 탭도 동일한 키보드 탐색·뒤로가기·인쇄 규칙을 적용합니다. 실제 접수·게시·예약을 실행하지 않는 설명용 화면입니다.
