---
name: ai-native-sdlc
description: 기능 개발, 버그 수정, 리팩터링, 프로젝트 문서 수정, 데이터 이행과 배포를 변경 영향에 맞춰 진행한다. 필요한 단계만 골라 결정과 검증 근거를 연결한다.
---

# AI-Native SDLC

- 요청 범위, 프로젝트 지침, 기존 계약과 테스트를 확인한다. 설명과 리뷰 요청은 해당 조사와 보고로 마친다.
- [단계 선택 기준](references/lifecycle.md)과 [작업 예시](references/compact-routes.md)를 바탕으로 변경 영향, 불확실성, 복구 난이도에 맞는 단계만 고른다. 단계 번호는 플레이북 식별자다. 선택한 단계는 합쳐 진행할 수 있고, 새 영향이 드러나면 필요한 단계만 추가한다.
- 기대 동작과 범위가 명확하면 수정과 검증으로 바로 진행한다. 중요한 미결은 [인터뷰 규칙](references/planning-interview.md)에 따라 확인한다. 범위가 같은 기존 결정은 재사용한다.
- 선택한 단계의 [종료 조건](references/lifecycle.md#단계별-종료-조건)을 적용한다. 동작 변경은 변경 전후 근거와 관련 회귀 결과를 확보한다. 동작을 바꾸지 않는 문서 수정은 내용과 링크 등 변경 부분을 확인한다. 필수 검사를 실행하지 못했으면 이유와 미검증 상태를 남긴다.
- 프로젝트가 쓰는 이슈, PR, 계약, 테스트와 문서를 우선한다. 별도 문서가 필요할 때 [산출물 구조](references/artifact-layout.md)를, 복잡한 관계를 설명하거나 검토할 때 [그림 규칙](references/diagram-policy.md)을 참고한다.
- 프로젝트의 권한과 승인 규칙을 따른다. 인수, 배포 정상, 운영 결과는 각각 판정한다.

## 마감 보고

- 기본은 작업 마지막에 채팅이나 기존 이슈·PR에 한 번 보고하는 것이다. 변경, 검증 결과와 근거, 미검증·차단 사항을 독자에게 맞는 말로 간단히 정리한다.
- 중요한 결정이나 승인이 필요하거나 진행이 막히면 중간에 공유한다. 사용자 요청이나 프로젝트 규칙에 따라 HTML 보고를 작성할 때만 [HTML 작성 가이드](references/stage-report.md)를 읽는다. 보고 시점과 범위도 해당 요청이나 규칙을 따른다.

출처 [DreambigOu/ELI5 원문](https://github.com/DreambigOu/ELI5/blob/main/skills/eli5/SKILL.md), [한국어 번역](references/eli5/SKILL.md), [MIT 라이선스](references/eli5/LICENSE)
