# Workflow Rules

이 문서는 `workflow/` 안의 문서들이 어떻게 연결되고 사용되는지 정리한다.

## Roles

- `ideas/`: 아직 task로 확정되지 않은 생각과 가능성을 관리한다.
- `issues/`: 아직 해결되지 않은 문제, 불편, 리스크를 관리한다.
- `tasks/`: 해야 할 일과 진행 중인 일을 관리한다.
- `work_logs/`: 실제로 한 작업과 그 결과를 기록한다.
- `decisions/`: 시도와 판단을 바탕으로 내린 결정을 기록한다.
- `templates/`: 새 문서를 만들 때 사용하는 템플릿을 둔다.

## Basic Flow

1. 아직 막연한 생각이면 먼저 `ideas/`에 아이디어를 만든다.
2. 해결해야 할 문제나 불편이면 먼저 `issues/`에 이슈를 만든다.
3. 실행할 가치가 분명해지면 `tasks/`에 작업을 만든다.
4. 실제로 무언가를 해보면 `work_logs/`에 작업 진행 기록을 남긴다.
5. 시도 결과를 바탕으로 방향을 정하면 `decisions/`에 결정을 남긴다.
6. 필요하면 task에서 관련 work log와 decision을 링크한다.

## Linking Rules

- idea는 관련 task를 가질 수 있다.
- issue는 관련 task와 decision을 가질 수 있다.
- task는 관련된 work log와 decision을 가질 수 있다.
- decision은 근거가 된 work log를 링크하는 것을 기본으로 한다.
- work log는 필요하면 관련 task를 링크할 수 있다.

## Status Rules

- 아직 시작하지 않은 작업은 `Next`에 둔다.
- 지금 진행 중인 작업은 `Now`에 둔다.
- 끝난 작업은 `Done`으로 옮긴다.

## Boundary

- `workflow/`는 `second brain`의 내용 영역이 아니라, 그 내용을 운영하는 메타 레이어다.
- 따라서 `workflow/` 안의 문서는 `1_active/`, `2_stable/`, `3_archive/` 흐름으로 자동 이동하지 않는다.
- `second brain` 주제 문서만 `0_inbox/`, `1_active/`, `2_stable/`, `3_archive/` 구조를 따른다.
- 필요하면 `workflow/`의 내용을 요약한 별도 문서를 `second brain` 쪽에 둘 수 있다.
