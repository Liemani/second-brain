---
created: 2026-06-28
---

# Agents

이 문서는 durable agent knowledge의 진입점입니다.

## Agent Knowledge

- durable agent knowledge는 역할과 운영 지식으로 구성된다.
- 이 지식은 반복 가능한 온보딩과 안정적인 수행을 위해 존재한다.
- `agents/roles/`는 역할의 장기 책임을, `agents/playbooks/`는 지속적인 운영 지식을 담는다.
- `AGENTS.md`는 온보딩용 부트스트랩을 담는다.

## Agents

- [roles](roles/index.md): long-lived role definitions
- [playbooks](playbooks/index.md): durable operational knowledge

## Boundaries

- Do not use this area to restate architectural decisions.
- Do not use role or playbook documents as session prompts.
- Keep the entry point focused on durable agent knowledge and navigation.
