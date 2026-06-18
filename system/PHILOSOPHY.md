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

- Objects는 실제 콘텐츠다.
- Schemas는 객체의 구조를 정의한다.
- Protocols는 모호하거나 반복되는 행동의 절차를 정의한다.
- Indexes는 관련 문서를 묶어 탐색을 돕는다.
- `system/`은 위 문서들을 모아 운영 레이어를 이룬다.

## Discoverability over Exhaustiveness

- `index.md`는 모든 파일을 나열하기보다 어디로 가야 하는지 알려주는 데 집중한다.
- 진입점은 완전한 목록이 아니라 적절한 출발점이어야 한다.

## Templates and Schemas

- templates는 문서를 작성하는 가이드다.
- schemas는 문서 구조를 설명한다.
- templates는 객체 그 자체가 아니다.
- schemas는 template 내용을 반복하지 않고 구조만 설명한다.

## Protocols Emerge from Ambiguity

- protocols는 행동이 모호하거나 결과가 엇갈릴 때 만든다.
- 자주 하는 일이라고 해서 protocol을 자동으로 만들지는 않는다.

## Indexes

- indexes는 관련 문서를 묶어 탐색을 돕는다.
- index는 목록이 아니라 탐색용 뷰다.

## Boundaries

- `areas/`는 주제와 결과물 성격의 자료를 담는다.
- `legacy/`는 이전 구조와 이전 자료를 보관한다.
- `system/`은 저장소 운영을 위한 문서를 담는다.
- `system/protocols/`는 공유 절차를 담는다.
- `system/templates/`는 작성용 구조를 담는다.

## Roles over Descriptions

- 객체는 무엇을 담는지보다 왜 존재하는지가 먼저 보여야 한다.
- role은 문서의 존재 이유와 책임을 드러낸다.

## Minimal Useful Structure

- 구조는 설명력이 있을 때만 추가한다.
- 개념적으로 멋진 계층보다 실제로 유지 가능한 최소 구조를 우선한다.

## System Evolution

- 구조가 바뀌었다고 해서 PHILOSOPHY를 자동으로 바꾸지는 않는다.
- PHILOSOPHY는 재사용 가능한 설계 원칙이 발견될 때 갱신한다.
- 시스템은 스스로를 설명할 수 있어야 하며, 그 설명도 시간이 지나며 갱신될 수 있다.
- 상태는 canonical 문서 안에 남아 있어야 하며, source 문서만 읽어도 작업을 이어갈 수 있어야 한다.
