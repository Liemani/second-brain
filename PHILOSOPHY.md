# Philosophy

이 문서는 second brain의 설계 원칙과 그 변화 가능성을 설명한다.

## Canonical Ownership

- 정보는 한 곳에서만 canonical owner를 가져야 한다.
- 구조와 제약은 각 원본 문서에 남아 있어야 한다.

## System Layers

- Objects are knowledge containers.
- Schemas define object structure.
- Protocols describe shared procedures for ambiguous or repeatable actions.

## Discoverability over Exhaustiveness

- `/index.md`는 모든 파일을 나열하기보다 어디로 가야 하는지 알려주는 데 집중한다.
- 진입점은 완전한 목록이 아니라 적절한 출발점이어야 한다.

## Templates Are Not Objects

- templates는 객체를 만드는 데 쓰는 작성 가이드다.
- 실제 객체 문서와 templates는 같은 것이 아니다.

## Templates Optimize for Authoring

- templates는 문서를 작성하는 사람을 위한 안내문이다.
- schemas는 문서 구조를 설명하는 문서다.

## Schemas Define Structure

- schemas는 Frontmatter Fields, Body Sections, Conventions를 정의한다.
- schemas는 template 내용을 반복하는 문서가 아니다.

## Protocols Emerge from Ambiguity

- protocols는 행동이 모호하거나 반복 오류가 생길 때 만든다.
- 자주 일어나는 일이라고 해서 protocol을 자동으로 만들지는 않는다.

## Indexes Are Perspective-Based Navigation

- indexes는 공유된 관점 아래 문서를 묶는다.
- index는 고정된 객체 목록이 아니라 관점 기반 뷰에 가깝다.

## Boundaries

- `areas/`는 운영 문서가 아니라 주제와 결과물 성격의 자료를 담는다.
- `legacy/`는 이전 구조와 이전 자료를 보관한다.
- `protocols/`는 공유 절차를 담는다.
- `templates/`는 실제 객체가 아니라 작성용 구조를 담는다.

## Roles over Descriptions

- 객체는 무엇을 담는지보다 왜 존재하는지가 먼저 보여야 한다.
- role은 문서의 존재 이유와 책임을 드러낸다.

## Minimal Useful Structure

- 구조는 설명력이 있을 때만 추가한다.
- 개념적으로 멋진 계층보다 실제로 유지 가능한 최소 구조를 우선한다.

## System Evolution

- 구조가 바뀌면 설계 원칙도 함께 다듬을 수 있다.
- 시스템은 스스로를 설명할 수 있어야 하며, 그 설명도 시간이 지나며 갱신될 수 있다.
- 상태는 canonical 문서 안에 남아 있어야 하며, source 문서만 읽어도 작업을 이어갈 수 있어야 한다.
