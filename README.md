# AI-Native SDLC

`ai-native-sdlc`는 기능 개발, 버그 수정, 리팩터링, 데이터 이행, 배포에 사용하는 스킬입니다. 요청에서 요구사항, 설계, 구현 작업, 검증 결과까지 근거를 연결해 작업을 이어갈 수 있게 돕습니다.

## 어떻게 진행하나요?

- 요청 범위와 변경 영향을 보고 필요한 단계만 고릅니다. 작은 변경은 기존 이슈나 PR을 정본으로 재사용하되, 변경별 `index.md`에서 정본, 단계 선택과 생략 이유, 현재 상태와 검증 근거를 연결합니다.
- 공통 문서는 `docs/`, 변경별 기록은 `specs/<변경 ID>/`에 둡니다. 기존 프로젝트의 문서 루트는 보존합니다. 문서는 합칠 수 있지만 진입점은 생략하지 않습니다.
- 모든 문서는 결론부터 짧은 개요식으로 씁니다. 상세 내용은 정본 한 곳에 기록하고, `index.md`는 링크와 짧은 상태표로 제한합니다.
- 계약, 데이터, 권한, 배포 위험이 바뀌면 해당 설계와 검증을 추가합니다. 복잡한 관계는 필요에 따라 편집 가능한 다이어그램으로 설명합니다.
- 작업이 끝나면 변경과 검증 결과를 한 번 보고합니다. HTML 보고는 요청이나 프로젝트 규칙에 따라 작성합니다.

## 어디서 시작하나요?

스킬을 선택한 뒤 원하는 변경과 작업 범위를 알려주세요. 설계 검토처럼 일부 단계만 요청할 수도 있습니다.

- [스킬 진입점](ai-native-sdlc/SKILL.md)
- [단계별 적용 조건과 종료 조건](ai-native-sdlc/references/lifecycle.md)
- [작업 유형별 진행 예시](ai-native-sdlc/references/compact-routes.md)
- [프로젝트 산출물 구조](ai-native-sdlc/references/artifact-layout.md)
- [단계별 템플릿](ai-native-sdlc/assets/templates/)
- [HTML 보고서 작성 가이드](ai-native-sdlc/references/stage-report.md)
