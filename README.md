# maker-docs

배재대 스마트 ICT 메이커톤 **B-SANG** 팀 — 산림 재난 통합 모니터링 노드(ForestGuard) 문서 저장소입니다.

📖 **문서 사이트**: https://maker.silentdraft.dev/
📋 **진행 현황**: [이슈](https://github.com/PCU-super-maker/maker-docs/issues) · [프로젝트 보드](https://github.com/orgs/PCU-super-maker/projects/1)

## 구조

```
docs/
├── index.md                 # 소개
├── requirements/            # 요구사항 분석서 (1~10절)
├── progress.md              # 진행 현황 · 상태 규칙
└── contributing.md          # 문서 수정 방법
.github/
├── labels.yml               # 이슈 라벨 정의 (push 시 자동 동기화)
├── ISSUE_TEMPLATE/          # 요구사항 · 작업 이슈 템플릿
└── workflows/               # 문서 배포 · 라벨 동기화
```

## 로컬 미리 보기

```bash
pip install -r requirements.txt
mkdocs serve
```

`main`에 push하면 GitHub Actions가 GitHub Pages로 자동 배포합니다.
