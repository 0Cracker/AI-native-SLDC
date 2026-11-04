# 02 아키텍처와 시스템 검증 설계

- **입력** G1 요구·인수 조건, 공통 구조, 현행 코드와 계약.
- 경계, 서비스 책임, 의존성, 데이터·런타임·배포와 품질 위험의 변경을 식별한다.
- 기술 맥락에 현행 버전, 실행 환경, 주요 의존성, 저장소, 검사 환경과 품질 제약 중 이번 선택에 영향을 주는 항목을 기록한다.
- 영향 영역마다 [다이어그램](../diagram-policy.md)을 작성하거나 기존 그림을 참조한다. 경계도와 런타임 시퀀스는 확인할 질문에 맞춰 고른다.
- 대안별 사용자 영향, 운영 비용, 장애·복구 차이를 비교한다. 큰 절충은 [인터뷰](../planning-interview.md)로 확인한다.
- 시스템 검증 시나리오, 환경, 관측 지점과 실패 경로를 정한다. 사용자 결과 단위로 Increment와 선행 계약을 잡는다.
- **기록** [아키텍처 영향](../../assets/templates/02-architecture/architecture-view.md)을 `architecture/A001-*.md`처럼 경계나 구조 결정별로 작성한다. 관련 요구를 모두 연결한다. [컨텍스트 예시](../../assets/templates/02-architecture/system-context.mmd), 중요 결정의 [ADR](../../assets/templates/02-architecture/adr.md), [실험 기록](../../assets/templates/00-intake/spike-report.md), [테스트 명세](../../assets/templates/03-detailed-design/test-plan.md)를 참조한다.
- **전환** [G2](../lifecycle.md#단계별-종료-조건) 충족 후 03.
