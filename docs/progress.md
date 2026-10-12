# 진행 현황

요구사항 36개(기능 27 + 비기능 9)는 모두 **같은 ID의 GitHub 이슈**로 관리합니다. 상태는 프로젝트 보드 칸으로, 우선순위와 구성요소는 라벨로 구분합니다.

[:material-view-column: 프로젝트 보드 열기](https://github.com/orgs/PCU-super-maker/projects/1){ .md-button .md-button--primary }
[:material-format-list-checks: 이슈 목록](https://github.com/PCU-super-maker/maker-docs/issues){ .md-button }

## 한눈에 보기

아래 숫자는 GitHub에서 실시간으로 가져옵니다(수 분 캐시). 숫자를 누르면 해당 이슈 목록이 열립니다.

| 구분 | 남은 이슈 | 완료 |
| --- | --- | --- |
| 필수 (MVP) | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%ED%95%84%EC%88%98?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%ED%95%84%EC%88%98) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%ED%95%84%EC%88%98?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%ED%95%84%EC%88%98) |
| 권장 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EA%B6%8C%EC%9E%A5?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EA%B6%8C%EC%9E%A5) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EA%B6%8C%EC%9E%A5?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EA%B6%8C%EC%9E%A5) |
| 선택 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EC%84%A0%ED%83%9D?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EC%84%A0%ED%83%9D) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EC%84%A0%ED%83%9D?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EC%84%A0%ED%83%9D) |
| 노드 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EB%85%B8%EB%93%9C?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EB%85%B8%EB%93%9C) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EB%85%B8%EB%93%9C?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EB%85%B8%EB%93%9C) |
| 게이트웨이 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EA%B2%8C%EC%9D%B4%ED%8A%B8%EC%9B%A8%EC%9D%B4?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EA%B2%8C%EC%9D%B4%ED%8A%B8%EC%9B%A8%EC%9D%B4) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EA%B2%8C%EC%9D%B4%ED%8A%B8%EC%9B%A8%EC%9D%B4?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EA%B2%8C%EC%9D%B4%ED%8A%B8%EC%9B%A8%EC%9D%B4) |
| 서버 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EC%84%9C%EB%B2%84?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EC%84%9C%EB%B2%84) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EC%84%9C%EB%B2%84?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EC%84%9C%EB%B2%84) |
| 위험도 엔진 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EC%9C%84%ED%97%98%EB%8F%84%EC%97%94%EC%A7%84?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EC%9C%84%ED%97%98%EB%8F%84%EC%97%94%EC%A7%84) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EC%9C%84%ED%97%98%EB%8F%84%EC%97%94%EC%A7%84?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EC%9C%84%ED%97%98%EB%8F%84%EC%97%94%EC%A7%84) |
| 웹 대시보드 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EB%8C%80%EC%8B%9C%EB%B3%B4%EB%93%9C?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EB%8C%80%EC%8B%9C%EB%B3%B4%EB%93%9C) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EB%8C%80%EC%8B%9C%EB%B3%B4%EB%93%9C?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EB%8C%80%EC%8B%9C%EB%B3%B4%EB%93%9C) |
| 비기능 | [![남음](https://img.shields.io/github/issues-raw/PCU-super-maker/maker-docs/%EB%B9%84%EA%B8%B0%EB%8A%A5?label=%EB%82%A8%EC%9D%8C&color=orange)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aopen+label%3A%EB%B9%84%EA%B8%B0%EB%8A%A5) | [![완료](https://img.shields.io/github/issues-closed-raw/PCU-super-maker/maker-docs/%EB%B9%84%EA%B8%B0%EB%8A%A5?label=%EC%99%84%EB%A3%8C&color=brightgreen)](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+is%3Aclosed+label%3A%EB%B9%84%EA%B8%B0%EB%8A%A5) |

## 상태 규칙

| 상태 | 보드 칸 | 언제 |
| --- | --- | --- |
| 할 일 | `Todo` | 이슈가 만들어지면 자동으로 들어감 |
| 진행 중 | `In Progress` | 담당자가 작업을 시작할 때 직접 옮김 |
| 막힘 | `Blocked` | 부품 대기, 다른 작업 의존 등으로 멈췄을 때. 이유를 댓글로 남김 |
| 완료 | `Done` | 이슈 본문의 완료 조건을 모두 체크하고 이슈를 닫으면 자동으로 옮겨짐 |

- 이슈를 맡으면 **Assignees**에 자기 이름을 넣습니다.
- 커밋 메시지나 PR에 `#이슈번호`를 적으면 이슈에 기록이 연결되고, `close #12`처럼 쓰면 병합 시 자동으로 닫힙니다.
- 우선순위를 바꿀 때는 이슈 라벨과 [기능 요구사항](requirements/functional.md) 표를 함께 고칩니다.

## 라벨

| 종류 | 라벨 |
| --- | --- |
| 유형 | `기능` `비기능` |
| 구성요소 | `노드` `게이트웨이` `서버` `위험도엔진` `대시보드` |
| 우선순위 | `필수` `권장` `선택` |

??? info "프로젝트 보드 처음 만들기 (관리자 1회)"
    1. 조직 페이지 → **Projects** → **New project** → 템플릿 **Board** 선택, 이름은 `ForestGuard`.
    2. 보드 설정 → **Status** 필드에 `Blocked` 옵션 추가 (Todo / In Progress / Blocked / Done).
    3. 보드 메뉴 → **Workflows** → **Auto-add to project** 켜고 저장소 `maker-docs`, 필터 `is:issue` 지정.
    4. 같은 Workflows에서 **Item closed → Done**, **Item reopened → In Progress**가 켜져 있는지 확인.
    5. 기존 이슈 36개는 보드 하단 **+ Add item** → `#` 입력 후 `maker-docs` 이슈를 한꺼번에 추가.
    6. 보드 우측 상단 **⋯ → Settings → Visibility**를 Public으로 하면 팀원이 아닌 사람도 볼 수 있습니다.
