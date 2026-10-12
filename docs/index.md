---
hide:
  - navigation
---

# ForestGuard — 산림 재난 통합 모니터링 노드

저가형 IoT 센서 노드를 산림에 분산 배치해 **산불과 산사태 위험을 하나의 센서망으로 동시에 감지**하고, 지역별 위험도를 웹 지도에 표시하는 시스템입니다. 배재대 스마트 ICT 메이커톤 **B-SANG** 팀 프로젝트입니다.

<div class="grid cards" markdown>

-   :material-file-document-outline:{ .lg .middle } **요구사항 분석서**

    ---

    배경과 범위, 기능·비기능 요구사항, 위험도 판단 기준, 시연 시나리오까지.

    [:octicons-arrow-right-24: 바로 가기](requirements/index.md)

-   :material-progress-check:{ .lg .middle } **진행 현황**

    ---

    요구사항 36개를 GitHub 이슈로 관리합니다. 담당자와 상태는 프로젝트 보드에서 확인하세요.

    [:octicons-arrow-right-24: 현황 보기](progress.md)

-   :material-sitemap-outline:{ .lg .middle } **시스템 구성**

    ---

    센서 노드 → LoRa → 게이트웨이 → 서버 → 위험도 엔진 → 웹 대시보드.

    [:octicons-arrow-right-24: 구성도](requirements/architecture.md)

-   :material-pencil-outline:{ .lg .middle } **문서 수정하기**

    ---

    문서는 마크다운으로 관리합니다. 수정 방법과 이슈 사용 규칙을 정리했습니다.

    [:octicons-arrow-right-24: 기여 가이드](contributing.md)

</div>

## 팀 구성

| 이름 | 역할 | 담당 영역 |
| --- | --- | --- |
| 고희경 (팀장) | H/W 개발 | 센서 노드 회로, 노드 펌웨어 |
| 김태호 | 기획 | 요구사항 정의, 위험도 판단 기준, 발표 |
| 임동섭 | S/W 개발 | 게이트웨이, 서버, 위험도 엔진 |
| 조연우 | 디자인 | 웹 대시보드 UI, 발표 자료 |
