# Templates

이 디렉터리는 바로 복사해서 사용할 수 있는 문서 템플릿과 그 사용 원칙을 모아두는 곳입니다.

## Meta

- Scope: template 문서 전체

## Files

- [template-index.md](template-index.md): 주제별 인덱스 템플릿
- [dream.md](dream.md): 꿈일기 템플릿
- [thought.md](thought.md): 생각 템플릿
- [idea.md](idea.md): 아이디어 템플릿
- [issue.md](issue.md): 이슈 템플릿
- [work_log.md](work_log.md): 작업 기록 템플릿
- [task.md](task.md): 작업 템플릿
- [decision.md](decision.md): 결정 템플릿

## dream.md

- 꿈에서 기억나는 내용을 개별 문서로 남길 때 사용합니다.
- thoughts와 분리해서 관리하며, 나중에 thought나 idea로 이어질 수 있습니다.

## template-index.md

- 같은 주제의 item들을 한 곳에 묶어보는 인덱스를 만들 때 사용합니다.
- `thought`, `idea`, `issue`, `task`, `dream`, `work_log`, `decision` 같은 item을 함께 둘 수 있습니다.

## thought.md

- 아직 정리되지 않은 생각을 개별 문서로 남길 때 사용합니다.
- 이후 필요하면 idea나 issue로 연결할 수 있습니다.

## idea.md

- 아직 task로 올릴지 정하지 않은 생각을 개별 문서로 남길 때 사용합니다.
- 이후 필요하면 관련 task로 연결할 수 있습니다.

## issue.md

- 아직 해결되지 않은 문제, 불편, 리스크를 개별 문서로 남길 때 사용합니다.
- 이후 필요하면 관련 task나 decision으로 연결할 수 있습니다.

## work_log.md

- 어떤 설정, 적용, 실험, 조사 작업을 실제로 진행한 뒤 기록할 때 사용합니다.
- 성공한 경우뿐 아니라 실패한 경우도 남기는 것을 전제로 합니다.
- 기본적으로 날짜만 기록하고 시간은 적지 않습니다.

## task.md

- 하나의 작업을 개별 문서로 관리할 때 사용합니다.
- 실제 실행 단위는 task 내부의 `Checklist` 항목으로 관리합니다.
- 각 checklist 항목에는 상태와 함께 날짜를 붙이는 것을 기본으로 합니다.
- 상태, 생성일, 관련 기록, 관련 결정을 함께 둡니다.

## decision.md

- 하나의 결정을 개별 문서로 남길 때 사용합니다.
- 근거가 된 시도와 연결된 작업을 함께 링크합니다.

## Writing Rules

- `결과`를 가장 먼저 써서 문서를 열었을 때 상태를 바로 알 수 있게 합니다.
- `수행 절차`와 `검증`은 분리합니다.
- 실패한 시도도 삭제하지 말고 `결과 상세`에 남깁니다.
- 실제 토큰, 비밀번호, 비밀키 원문은 기록하지 않습니다.
