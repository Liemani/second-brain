---
created: "2026-06-11"
---
# index 배치 방식 결정

`workflow/` 안의 각 분류 인덱스를 어디에 둘지에 대한 결정 문서이다.

## 결정

각 분류의 인덱스는 별도 `index/` 폴더에 모으지 않고, 각 분류 폴더 안에 `index.md`로 둔다.

## 이유

- `records/tasks/`, `records/work_logs/`, `records/decisions/`, `records/ideas/`, `records/issues/`, `system/templates/`와 각 인덱스의 관계를 가장 직관적으로 보여준다.
- 특정 분류를 열었을 때 같은 위치에서 바로 `index.md`를 볼 수 있어 접근성이 좋다.
- 별도 `index/` 폴더를 두면 인덱스가 누구를 설명하는지 한 번 더 해석해야 해서 구조가 오히려 멀어진다.

## 영향

- `workflow/index.md`는 상위 진입점만 담당한다.
- 각 분류별 목록과 상태 관리는 각 폴더의 `index.md`에서 유지한다.
