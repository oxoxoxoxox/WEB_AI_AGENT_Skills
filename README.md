# WEB AI Agent Skills

개인 웹 프로젝트에서 AI와 함께 기획, 디자인, 개발, 디버깅, 리뷰를 진행할 때 사용하는 Markdown 가이드 모음입니다. 프로젝트가 생기면 필요한 가이드와 템플릿을 가져와 실제 요구사항에 맞게 수정합니다.

## 분야별 시작점

| 분야 | 문서 | 쓰는 시점 |
|---|---|---|
| 기획 | [기획 가이드](plan/README.md) | 아이디어를 사용자 문제와 MVP 범위로 정리할 때 |
| 디자인 | [웹 디자인 가이드](design/design-guide.md) | 화면 흐름, 토큰, 공통 컴포넌트를 정할 때 |
| 개발 | [개발 가이드](development/README.md) | 구현 계획을 코드로 옮길 때 |
| 디버깅 | [디버깅 가이드](debugging/README.md) | 버그와 실패 원인을 찾을 때 |
| 리뷰 | [리뷰 및 완료 확인](review/README.md) | 변경 사항을 점검하고 작업을 마칠 때 |
| 작업 기억 | [인수인계 가이드](memory/README.md) | 새 대화나 다른 AI에서 작업을 이어갈 때 |
| 외부 원문 | [Superpowers 자료 안내](references/README.md) | 상세 개발 방법론과 스킬 원문을 읽을 때 |

## 권장 사용 순서

1. [프로젝트 브리프](design/project-brief-template.md)를 복사해 목적, 사용자, 핵심 기능을 채웁니다.
2. `plan/README.md`로 MVP 범위를 정하고 `design/design-guide.md`로 UI 기준을 정합니다.
3. [구현 계획 양식](plan/implementation-plan-template.md)에 작업과 검증 방법을 적습니다.
4. 개발 중에는 `development/`, 문제가 생기면 `debugging/`를 참고합니다.
5. `review/`로 실제 결과를 확인하고 `memory/` 방식으로 다음 작업을 남깁니다.

간단한 수정은 필요한 부분만 사용합니다. 모든 요청에 전체 절차를 반복하지 않습니다.

## AI에게 사용하는 예시

```text
이 저장소의 AGENTS.md를 읽어줘.
이번에는 plan/README.md와 design/design-guide.md를 기준으로
내 아이디어의 MVP 범위와 첫 화면 구성을 함께 정리하자.
아직 코드 구현은 하지 마.
```

```text
기존 프로젝트의 지침과 디자인 토큰을 먼저 확인해줘.
이 라이브러리의 development/README.md와 review/README.md를 참고해서
요청한 기능을 구현하고 실제로 확인한 결과를 알려줘.
```

실제 프로젝트에서는 필요한 문서를 `docs/` 등에 복사하고, 그 프로젝트의 `AGENTS.md`에서 경로를 참조하세요. 이 저장소를 다른 폴더에 보관하는 것만으로 모든 AI에 자동 적용되지는 않습니다.

## 직접 관리하는 가이드와 Superpowers 원문

- `design/`, `plan/`, `development/`, `debugging/`, `review/`, `memory/`: 내 작업 방식에 맞게 수정하는 가이드와 템플릿입니다.
- `references/superpowers/`: upstream 특정 커밋의 원본 스냅샷입니다. 원문 안의 링크와 보조 파일을 유지하려고 원래 디렉터리 구조를 보존했습니다.
- 분야별 가이드에서 관련 Superpowers 원문으로 연결합니다. 원문을 여러 폴더에 복제하지 않습니다.
- 원문을 보관했지만 플러그인을 설치하거나 스크립트·훅을 실행하지는 않았습니다. 상세 적용 방법과 출처는 [자료 안내](references/README.md)를 확인하세요.

## 수정 원칙

범용 규칙은 이 저장소에서 개선하고, 프로젝트별 색상·기술 스택·기능·진행 기록은 해당 프로젝트에서 관리합니다. 개인 자료가 필요하면 Git에서 제외한 `local/`을 사용합니다. 외부 자료는 출처와 라이선스를 유지합니다.
