# Workflow Rules

이 문서는 작업 운영 문서들이 어떻게 연결되고 사용되는지 정리한다.

## Roles

- `thoughts/`: 문득 든 생각을 자유롭게 기록한다. idea나 issue로 이어질 수도 있지만, 그럴 필요는 없다.
- `ideas/`: 아직 task로 확정되지 않은 생각과 가능성을 관리한다.
- `issues/`: 아직 해결되지 않은 문제, 불편, 리스크를 관리한다.
- `tasks/`: 작업을 관리한다. 실제 실행 단위는 각 task 안의 checklist 항목으로 둔다.
- `work_logs/`: 실제로 한 작업과 그 결과를 기록한다.
- `decisions/`: 시도와 판단을 바탕으로 내린 결정을 기록한다.
- `templates/`: 새 문서를 만들 때 사용하는 템플릿을 둔다.

## Basic Flow

1. 아직 막연하지만 가능성으로 보고 싶으면 `ideas/`에 아이디어를 만든다.
2. 해결해야 할 문제나 불편이면 `issues/`에 이슈를 만든다.
3. 실제 작업은 `tasks/`에 만든다.
4. 세부 실행 항목은 각 task 안의 checklist로 관리한다.
5. 실제로 무언가를 해보면 `work_logs/`에 작업 진행 기록을 남긴다.
6. 시도 결과를 바탕으로 방향을 정하면 `decisions/`에 결정을 남긴다.
7. 필요하면 task에서 관련 work log와 decision을 링크한다.

## Linking Rules

- idea는 관련 task를 가질 수 있다.
- thought는 필요하면 관련 idea나 issue를 가질 수 있다.
- issue는 관련 task와 decision을 가질 수 있다.
- task는 checklist, work log, decision을 함께 관리한다.
- decision은 근거가 된 work log를 링크하는 것을 기본으로 한다.
- work log는 필요하면 관련 task를 링크할 수 있다.

## Status Rules

- 아직 시작하지 않은 작업은 `Backlog`에 둔다.
- 지금 진행 중인 작업은 `Now`에 둔다.
- 끝난 작업은 `Done`으로 옮긴다.

## Boundary

- 이 문서들은 현재 second brain의 핵심 작업 영역을 구성한다.
- `legacy/`와 `areas/`는 주제와 자료를 다루고, 여기의 문서들은 작업 운영 자체를 다룬다.
