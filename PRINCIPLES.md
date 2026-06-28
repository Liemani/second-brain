# Principles

> A workspace where humans and AI agents continuously collaborate through shared context.

## Purpose

- 이 Workspace는 사람과 AI가 공유된 문맥을 바탕으로 함께 작업하기 위해 존재한다.
- 모든 구조와 문서는 그 협업을 더 자연스럽고 지속 가능하게 만드는 방향으로 유지한다.
- 아래 원칙은 구현보다 오래 유지되어야 하는 기준을 정의한다.

## Canonical Ownership

- 정보는 한 곳에서만 canonical owner를 가져야 한다.
- 각 문서는 자기 책임만 가진다.
- 설명과 구조는 가능한 한 원본 문서에 남아 있어야 한다.
- 저장소의 항목은 현재 운영과 관리에 충분한 이유가 있을 때만 남긴다.

## System Layers

- `agents/`는 durable agent knowledge를 담는다.
- `projects/`는 관리 중인 프로젝트와 그에 필요한 맥락, 책임을 담는다.
- `records/`는 판단이 끝난 지식, 결정, 경과를 담는다.
- `indexes/`는 탐색을 돕는다.
- `PRINCIPLES.md`는 저장소 운영 원칙을 담는다.
- `legacy/`는 보관할 옛 자료를 담는다.

## Workspace over Storage

- 이 저장소는 자료를 쌓아두는 곳이 아니라 함께 다루는 작업 공간이다.
- 남길 내용은 보관 가치보다 현재와 가까운 관리 필요성을 먼저 가져야 한다.
- 저장은 목적이 아니라 작업을 더 잘 유지하기 위한 수단이다.

## Discoverability over Exhaustiveness

- 진입 문서는 모든 파일을 나열하기보다 어디로 가야 하는지 알려주는 데 집중한다.
- 출발점은 완전한 목록이 아니라 적절한 탐색의 시작이어야 한다.

## Templates

- 템플릿은 필요한 문맥을 스스로 제공해야 한다.
- 각 템플릿은 무엇을 만들지와 어떻게 만들지를 함께 설명한다.

## Boundaries

- 각 영역은 책임을 분리해 같은 문서가 여러 역할을 동시에 떠안지 않게 한다.
- 기록은 기록답게, 탐색은 탐색답게, 운영은 운영답게 남긴다.
- 오래된 자료는 현재 구조와 섞지 않고 따로 보관한다.

## Context over Skills

- 이 시스템은 skill 기반 제어를 지향하지 않는다.
- 특정 행동을 위한 순차적인 절차 문서 집합을 만드는 것을 목표로 하지 않는다.
- agent는 필요한 문서를 읽으며 문맥을 형성하고, 그 문맥 안에서 자연스럽게 다음 행동을 결정해야 한다.
- 각 문서는 해야 할 일을 직접 지시하기보다 자신의 역할과 목적을 드러내야 한다.
- 시스템은 명령 집합보다 문맥 형성을 통해 동작하도록 지속적으로 유지한다.

## Roles over Descriptions

- 역할 문서는 `agents/roles/`에, playbook은 `agents/playbooks/`에 둔다.
- 기록 문서는 무엇을 담는지보다 왜 존재하는지가 먼저 보여야 한다.
- role은 문서의 존재 이유와 책임을 드러낸다.

## Minimal Useful Structure

- 구조는 설명력이 있을 때만 추가한다.
- 개념적으로 멋진 계층보다 실제로 유지 가능한 최소 구조를 우선한다.

## System Evolution

- PRINCIPLES는 구조 변경만으로 자동으로 수정하지 않는다.
- 재사용 가능한 설계 원칙이 발견될 때 갱신한다.
- 시스템은 스스로를 설명할 수 있어야 하며, 그 설명도 함께 진화한다.
