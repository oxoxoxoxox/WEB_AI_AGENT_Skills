# 한국어 글쓰기와 문서 교정

[DaleSeo/korean-skills](https://github.com/DaleSeo/korean-skills)의 스킬 3개를 이 저장소의 `.agents/skills/`에 설치했습니다. Superpowers 참고 자료와 달리 Codex가 프로젝트 스킬로 발견하는 위치에 배치했습니다. 정확한 버전은 [설치 기록](../.agents/skills/KOREAN_SKILLS_SOURCE.md)을 확인하세요.

## 스킬 선택

| 스킬 | 쓸 때 | 원문 |
|---|---|---|
| humanizer | 번역투·과장·불필요한 표현을 줄일 때 | [SKILL.md](../.agents/skills/humanizer/SKILL.md) |
| grammar-checker | 맞춤법·띄어쓰기·문법을 점검할 때 | [SKILL.md](../.agents/skills/grammar-checker/SKILL.md) |
| style-guide | 용어·말투·숫자·날짜 표기를 맞출 때 | [SKILL.md](../.agents/skills/style-guide/SKILL.md) |

전체 윤문은 humanizer → grammar-checker → style-guide 순서로 진행합니다. 맞춤법만 요청한 경우 grammar-checker만 적용합니다. 코드 작업이나 일반 대화에 세 스킬을 매번 실행하지 않습니다.

## Codex에서 사용하기

```text
$humanizer README의 의미와 기술 용어를 유지하면서 자연스럽게 다듬어줘.
$grammar-checker 기획서의 맞춤법과 띄어쓰기만 확인해줘.
$style-guide 이 문서들의 사용자/유저 표기와 말투를 통일해줘.
```

일반 문장으로 요청할 수도 있습니다. 설치한 스킬이 목록에 나타나지 않으면 새 대화를 시작하거나 Codex를 재시작하세요. Claude의 `/korean-skills:...` 명령을 그대로 복사할 필요는 없습니다.

## 프로젝트에 가져가기

필요한 스킬 폴더를 `SKILL.md` 하나만이 아니라 `references/`, `examples/`, `LICENSE`까지 통째로 해당 프로젝트의 `.agents/skills/`로 복사합니다. 설치 기록도 보존하고, 프로젝트의 `AGENTS.md`에서 이 글쓰기 규칙을 참조합니다. 같은 이름의 전역 스킬이 있는지 확인해 중복을 피합니다.

이 라이브러리에 설치했다고 다른 모든 프로젝트나 일반 웹 ChatGPT에 자동으로 설치되지는 않습니다. 전역 설치와 외부 앱 연결은 별도 작업입니다.

## 사실과 작성자 의도 보존

- 수치, 날짜, 이름, 기술명, 코드, URL, 직접 인용과 핵심 주장을 보존합니다.
- 작성자 목소리와 문서 목적을 유지합니다. 요청하지 않은 경력·성과·기술 수준을 추가하지 않습니다.
- 자연스럽게 만들기 위해 맞춤법을 일부러 틀리지 않습니다.
- 사용자·프로젝트의 표기 규칙과 적용되는 상위 지침이 일반적인 문체 권장보다 우선합니다.
- 규범상 오류와 문체 권장을 구분하고 애매한 제안은 단정하지 않습니다.
- 원본의 자연도 등급과 AI 작문 신호는 편집 참고 기준입니다. 작성 주체 판정이나 탐지 회피 성공을 보장하는 수치로 사용하지 않습니다.

원본의 `Read`, `Write`, `Edit`, `Grep`, `Glob`, `AskUserQuestion`은 현재 Codex의 파일·검색·질문 기능으로 해석합니다. `allowed-tools`가 새로운 도구나 권한을 부여하지 않습니다.

## 원본 관리

스킬 본문은 유지하고, 개인 작업 방식은 이 가이드에서 수정합니다. 원본의 잘못된 상대경로 한 곳은 수정했고 설치 기록에 명시했습니다. 각 폴더에 upstream MIT 라이선스를 포함했습니다. 이번 적용은 프로젝트 범위의 파일 설치이며 Claude 플러그인이나 MCP 서버 설치가 아닙니다. 파일 구조·참고 링크·두 저장소 간 일치 여부를 검증하고, 실제 자동 선택은 다음 Codex 사용 시 확인합니다.
