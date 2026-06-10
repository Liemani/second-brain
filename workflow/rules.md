# Workflow Rules

이 문서는 `workflow/` 안의 문서들이 어떻게 연결되고 사용되는지 정리한다.

## Roles

- `tasks/`: 해야 할 일과 진행 중인 일을 관리한다.
- `attempts/`: 실제로 시도한 내용과 그 결과를 기록한다.
- `decisions/`: 시도와 판단을 바탕으로 내린 결정을 기록한다.
- `templates/`: 새 문서를 만들 때 사용하는 템플릿을 둔다.

## Basic Flow

1. 새로운 일이 생기면 먼저 `tasks/`에 작업을 만든다.
2. 실제로 무언가를 해보면 `attempts/`에 시도 기록을 남긴다.
3. 시도 결과를 바탕으로 방향을 정하면 `decisions/`에 결정을 남긴다.
4. 필요하면 task에서 관련 attempt와 decision을 링크한다.

## Linking Rules

- task는 관련된 attempt와 decision을 가질 수 있다.
- decision은 근거가 된 attempt를 링크하는 것을 기본으로 한다.
- attempt는 필요하면 관련 task를 링크할 수 있다.

## Status Rules

- 아직 시작하지 않은 작업은 `Next`에 둔다.
- 지금 진행 중인 작업은 `Now`에 둔다.
- 끝난 작업은 `Done`으로 옮긴다.

## Boundary

- `workflow/`는 `second brain`의 내용 영역이 아니라, 그 내용을 운영하는 메타 레이어다.
- 따라서 `workflow/` 안의 문서는 `1_active/`, `2_stable/`, `3_archive/` 흐름으로 자동 이동하지 않는다.
- `second brain` 주제 문서만 `0_inbox/`, `1_active/`, `2_stable/`, `3_archive/` 구조를 따른다.
- 필요하면 `workflow/`의 내용을 요약한 별도 문서를 `second brain` 쪽에 둘 수 있다.
