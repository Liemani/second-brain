# project-template

이 저장소는 새 프로젝트를 만들 때 그대로 복제해서 사용하는 템플릿입니다.
이름 그대로, 새 프로젝트를 생성할 때 출발점으로 쓰는 구조입니다.
`project-name/`은 Git으로 관리되는 프로젝트 본체이고, `raw/`는 Git에 넣지 않을 외부 원본 파일을 따로 모으기 위한 구역입니다.

## Structure

- `raw/`
  - `inbox/`: 아직 분류하지 않은 유입 원문 파일
  - `original/`: 최종 보관할 원본 파일
  - `assets/`: 이미지 등 보조 자산 파일
- `project-name/`
  - 실제 프로젝트 생성 시 프로젝트명으로 바뀌는 루트 디렉터리
  - `README.md`: 프로젝트용 안내 문서
  - `memory/`: 작업 메모리와 운영 문서

세부 구조와 운영 방식은 `project-name/README.md`와 `project-name/memory/` 아래 문서를 참고합니다.
