# 기여 가이드

문서는 `docs/` 폴더의 마크다운 파일로 관리하고, `main` 브랜치에 반영되면 GitHub Actions가 사이트를 자동으로 다시 배포합니다(1~2분).

## 빠르게 고치기 (브라우저)

1. 고칠 페이지 우측 상단의 :material-file-edit-outline: **편집** 아이콘을 누릅니다.
2. GitHub 편집 화면에서 내용을 고치고 **Commit changes**를 누릅니다.
3. 1~2분 뒤 사이트에 반영됩니다.

## 로컬에서 미리 보기

```bash
git clone https://github.com/PCU-super-maker/maker-docs.git
cd maker-docs
pip install -r requirements.txt
mkdocs serve
```

브라우저에서 <http://127.0.0.1:8000> 을 열면 저장할 때마다 바로 반영됩니다.

## 새 페이지 추가

1. `docs/` 아래에 `.md` 파일을 만듭니다. (예: `docs/meetings/2026-10-15.md`)
2. `mkdocs.yml`의 `nav:`에 경로를 추가합니다.

## 작성 규칙

- 요구사항 ID(`FR-N01`, `NFR-03` 등)는 바꾸지 않습니다. 이슈 제목과 문서가 이 ID로 연결됩니다.
- 요구사항을 **추가**할 때는 다음 번호를 쓰고, 같은 ID로 이슈도 만듭니다(이슈 템플릿 "요구사항" 사용).
- 요구사항을 **삭제**할 때는 표에서 지우지 말고 우선순위를 `제외`로 바꾼 뒤, 이슈는 `not planned`로 닫습니다.
- 다이어그램은 ` ```mermaid ` 코드 블록으로 그립니다.
- 수식은 `$$ ... $$`(블록) 또는 `\( ... \)`(인라인)로 씁니다.
- 커밋 메시지 예: `docs: FR-W05 우선순위 권장→필수`, `docs: 하드웨어 부품 확정 (#14)`
