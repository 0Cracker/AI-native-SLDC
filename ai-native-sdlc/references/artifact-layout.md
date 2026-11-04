# 프로젝트 산출물 규칙

- 저장소 지침과 기존 문서로 공통 문서 루트, 변경별 명세 루트를 각각 찾는다. 정본이 모호하거나 기존 문서를 옮겨야 하면 먼저 확인한다.
- 기존 루트와 변경 ID를 재사용한다. 루트가 없으면 `docs/`와 `specs/`, 변경 ID가 없으면 `F001-short-slug`를 기본으로 쓴다.
- 같은 변경은 같은 폴더에서 이어간다. 문서 내부에서 Increment를 `INC-01`처럼 구분한다. 신규 파일명은 소문자와 하이픈을 사용하고 기존 ID와 계약 형식을 보존한다.

## 기본 폴더

```text
docs/
├── product.md, constitution.md, architecture.md, tech-stack.md, glossary.md
├── decisions/ADR-*.md
└── diagrams/
specs/F001-short-slug/
├── index.md
├── intake.md
├── requirements/
│   └── R001-short-slug.md
├── architecture/
│   ├── A001-short-slug.md
│   └── diagrams/
├── designs/
│   ├── D001-short-slug.md
│   └── diagrams/
├── contracts/
├── tests/test-plan.md, tests/golden/
├── tasks.md
├── tasks/T001-short-slug.md
├── verification.md
├── spike-report.md
├── release.md
├── operations.md
└── reports/
```

| 경로 | 정본과 생성 시점 |
|---|---|
| `index.md` | 관계 지도, Increment와 Gate 판정. 본문은 각 정본에 기록 |
| `intake.md` | 00 요청, 목표, 범위, 성공 기준과 주요 결정 |
| `requirements/R001-*.md` | 01 요구 하나, 시나리오, 인수 조건과 기대값 근거. Intake와 관련 요구 연결 |
| `architecture/A001-*.md` | 02 영향을 받는 경계나 구조 결정 하나. 관련 요구와 구조 의존성 연결 |
| `designs/D001-*.md` | 03 구현·검증할 상세 설계 단위 하나. 관련 구조 결정과 요구·검사 연결 |
| `architecture/diagrams/A001-*.mmd`, `designs/diagrams/D001-*.mmd` | 단계별 편집 가능한 그림 원본. 공통 그림은 공통 문서 루트 |
| `contracts/` | 변경 API·이벤트·Tool의 정형 계약 또는 기존 정본 참조 |
| `tests/test-plan.md`, `tests/golden/` | 검증 명세, 필요시 허용된 독립 기대값. 실행 테스트는 저장소의 기존 경로 |
| `tasks.md` | G4 작업 계획과 의존성. 05에서 상태와 근거 링크 갱신 |
| `tasks/<task-id>-<slug>.md` | G5 작업별 구현·결정·인계 기록. 변경 이력이나 인계를 별도로 추적할 때만 작성 |
| `verification.md` | G5 실행 증거와 판정, 06a 통합, 06b 인수 결과의 정본 |
| `spike-report.md`, 공통 `decisions/ADR-*.md` | 실험 기록, 중요한 구조 결정 |
| `release.md`, `operations.md` | 07 배포·복구, 08 운영 관측과 결정. 적용 시 작성 |
| `reports/<stage>-<scope>-<round>.html` | 단계 마감 시점의 요약. 기존 경로를 우선하고 [보고 규칙](stage-report.md)을 따른다. |

- 신규 변경은 위 구조를 기본으로 한다. 기존 변경의 정본과 ID는 재사용한다. 필요한 폴더와 문서만 만들고 이관은 먼저 확인한다.
- 요구는 인수 판단 단위, 아키텍처는 경계·구조 결정 단위, 상세 설계는 동작·계약 단위로 나눈다. 03의 A~H와 확장 영역 이름은 `A001`·`D001` 같은 문서 ID와 구분한다.
- 각 문서가 상위 근거를 ID와 상대 링크로 가리킨다. 한 문서에서 여러 상위 근거를 참조할 수 있다. 관계 지도에는 상위 근거와 후속 문서를 찾아가는 링크만 기록한다.
- 작성 틀은 [단계별 플레이북](lifecycle.md), [03 세부 가이드](playbooks/03-detailed-design.md)에서 고른다. [작성 근거와 한국어 규칙](template-sources.md)을 참고한다.
