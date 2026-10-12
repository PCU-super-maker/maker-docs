# 5. 비기능 요구사항

아래 목표치는 팀 합의를 위한 초안이며, 시연 환경에서 측정 가능한 값으로 정했다. 합의된 값은 이 표와 해당 이슈에 함께 반영한다.

| ID | 분류 | 요구사항 | 목표치 (초안) | 이슈 |
| --- | --- | --- | --- | --- |
| `NFR-01` | 성능 | 센서 측정부터 대시보드 표시까지 지연 | 일반 데이터 10초 이내, 화재 경보 5초 이내 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-01%22+in%3Atitle) |
| `NFR-02` | 성능 | 정기 측정·송신 주기 | 시연 모드 10초, 운영 모드 10분 (설정 변경 가능) | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-02%22+in%3Atitle) |
| `NFR-03` | 신뢰성 | 시연 중 패킷 수신율 | 실내·근거리 기준 95% 이상 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-03%22+in%3Atitle) |
| `NFR-04` | 신뢰성 | 센서 1종 고장 시에도 나머지 센서값은 정상 송신 | 센서별 오류값을 별도 표기 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-04%22+in%3Atitle) |
| `NFR-05` | 전력 | 노드의 배터리 단독 동작 | 시연 시간(최소 8시간) 동안 무충전 동작 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-05%22+in%3Atitle) |
| `NFR-06` | 확장성 | 코드 수정 없이 노드 추가 | 노드 등록만으로 지도에 표시 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-06%22+in%3Atitle) |
| `NFR-07` | 보안 | 게이트웨이→서버 전송 인증 | API 키 기반 인증 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-07%22+in%3Atitle) |
| `NFR-08` | 사용성 | 위험 등급의 직관적 구분 | 4단계 색상 + 텍스트 병기 (색각 이상 고려) | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-08%22+in%3Atitle) |
| `NFR-09` | 유지보수 | 위험도 판단 기준값 분리 | 임계값을 설정 파일로 관리해 재배포 없이 조정 | [보기](https://github.com/PCU-super-maker/maker-docs/issues?q=is%3Aissue+%22NFR-09%22+in%3Atitle) |
