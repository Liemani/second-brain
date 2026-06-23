# Philosophy

이 문서는 저장소를 유지하는 설계 원칙을 정리하고, 시스템이 바뀔 때 함께 갱신된다.

## Purpose

- 이 저장소가 어떤 원칙으로 구성되고 유지되어야 하는지 설명한다.
- 구조가 바뀌더라도 무엇을 지켜야 하는지, 어떤 기준으로 문서와 레이어를 해석해야 하는지 남긴다.
- source 문서만 읽어도 작업을 이어갈 수 있도록, 운영 레이어의 공통 기준을 제공한다.

## Canonical Ownership

- 정보는 한 곳에서만 canonical owner를 가져야 한다.
- 각 문서는 자기 책임만 가진다.
- 설명과 구조는 가능한 한 원본 문서에 남아 있어야 한다.

## System Layers

- `records/`는 실제 기록 문서를 담는다.
- 각 `records/*/template.md`와 `indexes/template.md`는 기록 문서와 index 문서를 쓰는 표면과 가이드를 함께 담는다.
- `indexes/`는 관련 문서를 묶어 탐색을 돕는다.
- `system/`은 위 문서들을 모아 운영 레이어를 이룬다.

## Discoverability over Exhaustiveness

- `index.md`는 모든 파일을 나열하기보다 어디로 가야 하는지 알려주는 데 집중한다.
- 진입점은 완전한 목록이 아니라 적절한 출발점이어야 한다.

## Templates

- template 파일은 문서를 작성하는 표면이다.
- 각 template는 실제로 복사할 본문과 그 본문을 해석하는 가이드를 함께 담는다.
- template 파일은 기록 문서 그 자체가 아니다.

## Indexes

- indexes는 관련 문서를 묶어 탐색을 돕는다.
- index는 목록이 아니라 탐색용 뷰다.

## Boundaries

- `records/`는 실제 기록 문서를 담는다.
- `records/*/template.md`는 각 기록 컬렉션과 함께 둔다.
- `indexes/`는 저장소 전체를 탐색하는 문서를 담고 `records/` 밖에 남는다.
- `areas/`는 주제와 결과물 성격의 자료를 담는다.
- `legacy/`는 이전 구조와 이전 자료를 보관한다.
- `system/`은 저장소 운영을 위한 문서를 담는다.
- `system/template_guide.md`는 템플릿 구조와 가이드를 설명한다.

## Context over Skills

- 이 시스템은 skill 기반 제어를 지향하지 않는다.
- 특정 행동을 위한 순차적인 절차 문서 집합을 만드는 것을 목표로 하지 않는다.
- agent는 필요한 문서를 읽으며 문맥을 형성하고, 그 문맥 안에서 자연스럽게 다음 행동을 결정해야 한다.
- 각 문서는 해야 할 일을 직접 지시하기보다 자신의 역할과 목적을 드러내야 한다.
- 시스템은 명령 집합보다 문맥 형성을 통해 동작하도록 지속적으로 유지한다.

## Roles over Descriptions

- 기록 문서는 무엇을 담는지보다 왜 존재하는지가 먼저 보여야 한다.
- role은 문서의 존재 이유와 책임을 드러낸다.

## Minimal Useful Structure

- 구조는 설명력이 있을 때만 추가한다.
- 개념적으로 멋진 계층보다 실제로 유지 가능한 최소 구조를 우선한다.

## System Evolution

- 구조가 바뀌었다고 해서 PHILOSOPHY를 자동으로 바꾸지는 않는다.
- PHILOSOPHY는 재사용 가능한 설계 원칙이 발견될 때 갱신한다.
- 시스템은 스스로를 설명할 수 있어야 하며, 그 설명도 시간이 지나며 갱신될 수 있다.
- 상태는 canonical 문서 안에 남아 있어야 하며, source 문서만 읽어도 작업을 이어갈 수 있어야 한다.
