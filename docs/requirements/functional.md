# 4. 기능 요구사항

기능 요구사항은 구성요소 5개에 걸쳐 27개이며, 이 중 **필수(MVP) 15개**가 메이커톤 시연의 최소 완성 범위다. 각 요구사항은 같은 ID의 GitHub 이슈로 관리하며, 진행 상태는 [진행 현황](../progress.md)에서 확인한다.

!!! tip "우선순위를 바꾸려면"
    이 표와 해당 이슈의 우선순위 라벨(`필수`·`권장`·`선택`)을 **함께** 바꿔 주세요. 문서 수정 방법은 [기여 가이드](../contributing.md)에 있습니다.

| 우선순위 | 의미 |
| --- | --- |
| 필수 | MVP. 시연 시나리오 통과에 반드시 필요 |
| 권장 | 완성도를 높이는 기능. 필수 완료 후 진행 |
| 선택 | 시간이 남을 때 또는 향후 확장 |

## 4.1 노드 펌웨어

| ID | 요구사항 | 설명 | 우선순위 | 이슈 |
| --- | --- | --- | --- | --- |
| `FR-N01` | 센서 주기 측정 | 강우·토양 수분·기울기·온습도·연기/CO 5종을 정해진 주기로 측정한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-N01%22+in%3Atitle) |
| `FR-N02` | LoRa 송신 | 측정값을 노드 ID와 함께 패킷으로 묶어 게이트웨이로 송신한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-N02%22+in%3Atitle) |
| `FR-N03` | 이벤트 즉시 송신 | 기울기 급변 또는 연기/CO 임계 초과 시 주기와 무관하게 즉시 송신한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-N03%22+in%3Atitle) |
| `FR-N04` | 저전력 동작 | 측정 사이에 딥슬립으로 전력 소모를 줄인다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-N04%22+in%3Atitle) |
| `FR-N05` | 배터리 상태 보고 | 배터리 전압을 측정해 패킷에 포함한다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-N05%22+in%3Atitle) |

## 4.2 게이트웨이

| ID | 요구사항 | 설명 | 우선순위 | 이슈 |
| --- | --- | --- | --- | --- |
| `FR-G01` | 수신·서버 전달 | LoRa 패킷을 수신해 Wi-Fi로 서버에 전달한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-G01%22+in%3Atitle) |
| `FR-G02` | 패킷 검증 | 체크섬이 맞지 않거나 형식이 잘못된 패킷은 버린다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-G02%22+in%3Atitle) |
| `FR-G03` | 전송 실패 버퍼링 | 서버 연결이 끊기면 패킷을 임시 저장했다가 재전송한다 | 선택 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-G03%22+in%3Atitle) |

## 4.3 서버

| ID | 요구사항 | 설명 | 우선순위 | 이슈 |
| --- | --- | --- | --- | --- |
| `FR-S01` | 측정 데이터 저장 | 노드 ID, 수신 시각, 센서값을 DB에 저장한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-S01%22+in%3Atitle) |
| `FR-S02` | 노드 정보 관리 | 노드 ID, 위경도, 설치 지역을 등록·수정한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-S02%22+in%3Atitle) |
| `FR-S03` | 조회 API 제공 | 대시보드에 노드별 최신값과 기간별 이력을 제공한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-S03%22+in%3Atitle) |
| `FR-S04` | 통신 두절 판정 | 일정 시간 데이터가 오지 않은 노드를 두절 상태로 표시한다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-S04%22+in%3Atitle) |

## 4.4 위험도 엔진

| ID | 요구사항 | 설명 | 우선순위 | 이슈 |
| --- | --- | --- | --- | --- |
| `FR-R01` | 산불 위험 지수 산출 | 토양 수분·습도·강우 감소, 기온 상승을 반영해 노드별 지수를 계산한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-R01%22+in%3Atitle) |
| `FR-R02` | 산사태 위험 지수 산출 | 강우·토양 수분·기울기 변화 증가를 반영해 노드별 지수를 계산한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-R02%22+in%3Atitle) |
| `FR-R03` | 위험 등급 변환 | 각 지수를 정상·주의·경계·위험 4단계로 변환한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-R03%22+in%3Atitle) |
| `FR-R04` | 화재 감지 경보 | 연기/CO가 임계값을 넘으면 지수와 무관하게 즉시 화재 경보를 발생시킨다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-R04%22+in%3Atitle) |
| `FR-R05` | 지역별 집계 | 같은 지역 노드의 위험도를 묶어 지역 위험도를 산출한다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-R05%22+in%3Atitle) |

## 4.5 웹 대시보드

| ID | 요구사항 | 설명 | 우선순위 | 이슈 |
| --- | --- | --- | --- | --- |
| `FR-W01` | 위험 지도 | 지도 위에 노드 위치를 위험 등급 색으로 표시한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W01%22+in%3Atitle) |
| `FR-W02` | 노드 상세 | 노드 선택 시 센서 최신값, 산불·산사태 지수, 최종 수신 시각을 보여준다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W02%22+in%3Atitle) |
| `FR-W03` | 경보 표시 | 경계·위험 등급 또는 화재 감지 시 화면 알림을 띄우고 경보 목록에 기록한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W03%22+in%3Atitle) |
| `FR-W04` | 실시간 갱신 | 새로고침 없이 최신 데이터로 화면을 갱신한다 | 필수 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W04%22+in%3Atitle) |
| `FR-W05` | 센서 추이 그래프 | 노드별 센서값을 시간 축 그래프로 보여준다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W05%22+in%3Atitle) |
| `FR-W06` | 레이어 전환 | 산불 위험과 산사태 위험 지도를 전환해 볼 수 있다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W06%22+in%3Atitle) |
| `FR-W07` | 노드 상태 표시 | 통신 두절·배터리 부족 노드를 별도 표시한다 | 권장 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W07%22+in%3Atitle) |
| `FR-W08` | 경보 확인 처리 | 관제 담당자가 경보를 확인 처리하면 목록에서 상태가 바뀐다 | 선택 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W08%22+in%3Atitle) |
| `FR-W09` | 외부 알림 | 경보를 SMS·메신저로 관계 기관과 주민에게 전달한다 | 선택 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W09%22+in%3Atitle) |
| `FR-W10` | 모바일 대응 | 휴대폰 화면에서도 지도와 경보를 확인할 수 있다 | 선택 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22FR-W10%22+in%3Atitle) |

