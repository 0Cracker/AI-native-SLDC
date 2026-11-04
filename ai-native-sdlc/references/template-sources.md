# 템플릿 작성 근거

| 출처 | 반영한 구조 |
|---|---|
| [Kiro Requirements-First](https://kiro.dev/docs/specs/feature-specs/requirements-first/) | 요구와 인수 조건, 기술 설계와 그림, 구현 작업을 분리한다. |
| [Spec Kit 사양](https://github.com/github/spec-kit/blob/main/templates/spec-template.md), [계획](https://github.com/github/spec-kit/blob/main/templates/plan-template.md), [작업](https://github.com/github/spec-kit/blob/main/templates/tasks-template.md) | 우선순위가 있는 사용자 시나리오, 구현 환경과 제약, 독립적으로 확인할 작업 단위 및 의존성을 기록한다. |
| [Spec Kit 명세 체크리스트](https://github.com/github/spec-kit/blob/main/templates/commands/checklist.md) | 명세의 누락·모호성·충돌 판정과 제품의 실제 실행 결과를 구분한다. |
| Mavin 외, [Easy Approach to Requirements Syntax](https://ccy05327.github.io/SDD/08-PDF/Easy%20Approach%20to%20Requirements%20Syntax%20%28EARS%29.pdf), IEEE RE 2009 | 조건, 사건, 상태에 대응하는 시스템 반응을 한국어로 분명하게 쓰고, 정상과 예외의 기대 결과를 구분한다. |
| Kazman 외, [The Architecture Tradeoff Analysis Method](https://www.sei.cmu.edu/documents/196/1998_019_001_29711.pdf), 1998 | 품질 시나리오로 대안을 비교하고, 근거·절충·잔여 위험을 설계와 결정 기록에 남긴다. |
| Gotel과 Finkelstein, [An Analysis of the Requirements Traceability Problem](https://discovery.ucl.ac.uk/id/eprint/749/), 1994 | 요구의 출처를 남기고, 인수 조건에서 설계·작업·실행 증거까지 양방향으로 추적한다. |

## 한국어 작성 규칙

- 결정과 영향을 먼저 쓰고 조건, 예외, 판정 근거를 구분한다.
- 요구는 “유효한 조건으로 요청하면 시스템은 …을 반환한다”처럼 관찰 가능한 동작으로 쓴다.
- 파일명, API, 상태값, ID, 측정 단위는 기존 표기를 따른다.
- 미정 기준은 결정자와 질문을 기록한다. 원본은 ID나 링크로 참조하고 실제 값은 관측 또는 승인된 근거에서 가져온다.

## 추적 순서

요구 ID → 인수 조건 ID → 아키텍처·설계·계약 ID → Task·검사 ID → 대상 리비전의 실행 증거.
