---
created: "2026-06-10"
related_decisions:
  - "[2026-06-11_index_placement.md](../decisions/2026-06-11_index_placement.md)"
---
# workflow 구조 구축

`workflow/`를 루트 메타 레이어로 분리하고, 작업 운영에 필요한 기본 문서 구조를 정리한 작업 기록이다.

## 결과

`workflow/` 아래에 `tasks`, `work_logs`, `decisions`, `templates`와 각 진입 문서를 두는 구조를 만들었다.

## 환경

- 적용 대상: `second brain 저장소`
- 대상: `개인 작업 운영 체계`
- 방식: `디렉터리 분리, 링크 재정리, 템플릿 추가`

## 수행 절차

### 1. 운영 문서 분리

1. `1_active`에 있던 `tasks`, `work_logs`, `decisions`, `templates`를 식별했다.
2. 이 문서들이 현재 주제 문서가 아니라 운영용 메타 레이어라는 점을 정리했다.
3. 관련 문서와 디렉터리를 루트 `workflow/` 아래로 이동했다.

### 2. 진입점과 규칙 정리

1. `workflow/index.md`를 만들어 진입점을 만들었다.
2. `workflow`의 운영 제약을 정리하는 문서를 추가해 `task`, `work log`, `decision`의 역할과 흐름을 정리했다.
3. `workflow`는 `second brain` 내용 흐름과 별개라는 경계를 문서화했다.

### 3. 템플릿 보강

1. 기존 `work_log.md`를 유지했다.
2. `task.md`와 `decision.md` 템플릿을 추가했다.
3. 템플릿 인덱스에 각 문서의 역할을 정리했다.

## 결과 상세

- 기대한 결과: `second brain`의 내용 문서와 작업 운영 문서를 분리한 구조를 만들고 싶었다.
- 실제 결과: `workflow/`를 독립 루트로 두고, 운영 문서와 템플릿을 별도 체계로 정리했다.
- 문제 또는 실패 원인 후보: 아직 모든 task, work log, decision 사이의 상호 링크 규칙이 완전히 자동화된 것은 아니다.
- 다음 시도 아이디어: `task`에서 관련 `work log`, `decision` 링크를 더 일관되게 추가하고, 새 문서 생성 규칙을 더 다듬는다.
