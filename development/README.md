# 개발 가이드

## 구현 순서

1. 실제 프로젝트의 지침, 기술 스택, 기존 코드와 테스트를 확인합니다.
2. 요청한 동작과 완료 기준을 정리합니다. 복잡한 기능은 [구현 계획](../plan/implementation-plan-template.md)을 작성합니다.
3. 기존 디자인 토큰과 공통 컴포넌트를 재사용합니다.
4. 작고 검증 가능한 단위로 구현합니다. 요청과 무관한 정리 작업은 범위에 섞지 않습니다.
5. 변경에 맞는 테스트, 정적 검사, 빌드, 실제 실행을 수행합니다.
6. [리뷰 가이드](../review/README.md)로 결과를 확인하고 확인하지 못한 부분을 보고합니다.

동작 로직과 회귀 버그에는 의미 있는 테스트를 사용합니다. Superpowers의 TDD를 명시적으로 적용할 때는 해당 원문을 따릅니다. 문서 수정이나 단순 시각적 조정에 구현을 그대로 복제하는 테스트를 추가하지 않습니다.

## 작업 방식 선택

- 작은 작업은 한 에이전트가 순서대로 진행합니다.
- 여러 작업이 독립적이고 사용자·프로젝트 지침이 허용할 때 병렬 진행을 검토합니다.
- 분리된 브랜치가 필요하면 기존 변경을 보존하고 Git worktree 사용을 검토합니다.
- 커밋, 원격 반영, PR, 배포는 해당 작업의 사용자 요청 범위를 따릅니다.

## Superpowers 관련 원문

| 스킬 | 역할 |
|---|---|
| [test-driven-development](../references/superpowers/skills/test-driven-development/SKILL.md) | 실패 테스트부터 시작하는 구현 |
| [executing-plans](../references/superpowers/skills/executing-plans/SKILL.md) | 계획의 순차 실행 |
| [subagent-driven-development](../references/superpowers/skills/subagent-driven-development/SKILL.md) | 작업별 에이전트와 검토 |
| [dispatching-parallel-agents](../references/superpowers/skills/dispatching-parallel-agents/SKILL.md) | 독립 작업 병렬 진행 |
| [using-git-worktrees](../references/superpowers/skills/using-git-worktrees/SKILL.md) | 작업 공간 분리 |
| [finishing-a-development-branch](../references/superpowers/skills/finishing-a-development-branch/SKILL.md) | 검증 후 브랜치 마무리 |

이 폴더의 가이드는 개인 프로젝트용 자체 요약입니다. 원본 스킬을 수정하거나 공식 번역으로 배포한 것이 아닙니다.
