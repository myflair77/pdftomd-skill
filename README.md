# PDFtoMD

PDF를 요약하지 않고 원문 구조와 의미를 보존한 주제별 Markdown·Obsidian 노트로 변환하고 검수하는 Codex 스킬입니다.

## 설치

다른 컴퓨터의 Codex에서 다음과 같이 요청하세요.

```text
$skill-installer https://github.com/myflair77/pdftomd-skill/tree/main/skills/pdftomd 에 있는 스킬을 설치해 줘.
```

설치 후 다음 대화 차례부터 `$pdftomd`로 사용하세요. 목록에 나타나지 않으면 Codex를 다시 시작하세요.

## 사용

```text
$pdftomd 이 PDF를 조사하고 분할 방식과 시범 변환을 준비해 줘: <PDF 경로>
```

목차 기준 분할 또는 분량 균형 분할을 선택하고 시범 결과를 확인한 뒤 전체 변환을 진행합니다. 실제 작업에는 PDF 읽기·렌더링과 파일 작성이 가능한 실행 환경이 필요합니다. 이 저장소는 관련 프로그램을 자동 설치하지 않습니다.

## 배포 범위와 개인 데이터

배포 파일은 `skills/pdftomd/SKILL.md`, `agents/openai.yaml`, `references/`의 지침 파일뿐입니다. PDF, 변환 노트, 이미지, 개인 추천 이력은 포함하지 않습니다.

추천 기능의 기록 형식과 처리 규칙은 포함하지만 실제 이력은 없습니다. 사용 중 생성되는 `data/recommendation-history.jsonl`은 설치된 스킬 폴더의 개인 데이터이며 Git에서 제외합니다.

GitHub에 변경 사항을 올려도 이미 설치한 스킬이 자동으로 업데이트되지는 않습니다. 업데이트 시 개인 `data/`를 보존하고 지침 파일만 교체하세요.
