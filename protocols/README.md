# Protocols

이 디렉터리는 second brain에서 인간과 AI가 함께 따를 수 있는 공유 행동 프로토콜을 모아둔다.

## Meta

- Scope: protocol 문서 전체

## Purpose

- protocol은 객체를 어떻게 옮기고, 상태를 어떻게 바꾸고, 반복 가능한 작업을 어떤 순서로 수행할지 정하는 공유 절차다.
- protocol은 AI 지시문이 아니라, 인간과 AI가 함께 이해하고 따라갈 수 있는 합의된 행동 방식이다.

## What Protocols Are Not

- template가 아니다. template는 문서 형식이고, protocol은 행동 절차다.
- rule가 아니다. rule은 시스템 전반의 제약이고, protocol은 그 안에서 수행하는 구체적 절차다.
- command 문서가 아니다. 일회성 실행 지시가 아니라 반복 가능한 전환 규약이다.

## Current Scope

- 이 디렉터리는 현재 워크플로에서 이미 가능한 상태 전환과 반복 작업만 다룬다.
- 새 workflow를 발명하기보다, 기존 객체와 문서 사이의 이동 규칙을 명시하는 데 집중한다.

## Files

- [index.md](index.md): protocol 문서 인덱스
- [template.md](template.md): protocol 문서 템플릿
- [promote_idea_to_task.md](promote_idea_to_task.md): idea를 task로 올리는 프로토콜
- [create_work_log.md](create_work_log.md): work log를 만드는 프로토콜

## Notes

- protocol은 객체를 변화시키는 방식에 대한 합의다.
- object, protocol, rule의 관계는 `objects -> protocols -> rules` 순으로 이해한다.
