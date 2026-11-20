# 외부 자료와 Superpowers 원문

## 보관 방식

[obra/superpowers](https://github.com/obra/superpowers)의 특정 커밋을 `superpowers/`에 원래 구조 그대로 보관합니다. MD 외에 원문에서 참조하는 보조 자료·스크립트·설정도 포함하지만 실행하거나 플러그인으로 등록하지 않았습니다. Git 이력은 포함하지 않습니다.

정확한 버전과 라이선스는 [SUPERPOWERS_SOURCE.md](SUPERPOWERS_SOURCE.md)를 확인하세요. 원문은 [README](superpowers/README.md)와 [skills](superpowers/skills/)에서 읽을 수 있습니다.

분야별 입구는 `plan/`, `development/`, `debugging/`, `review/`에 있습니다. [using-superpowers](superpowers/skills/using-superpowers/SKILL.md)는 원본 사용 방법, [writing-skills](superpowers/skills/writing-skills/SKILL.md)는 스킬 제작 방법을 다룹니다.

## 내 방식으로 수정할 때

- 원본을 직접 바꾸기보다 분야별 가이드에서 내 절차를 정리합니다.
- 원본을 바꿔야 한다면 변경 파일과 이유를 별도로 기록합니다.
- 이 저장소의 분야별 가이드는 개인 프로젝트용으로 새로 쓴 문서이며, Superpowers 전체와 동일하게 작동하지는 않습니다.
- 실제 플러그인 설치는 upstream의 현재 설치 문서를 다시 확인하고 별도로 진행합니다.

## 원본을 업데이트할 때

1. upstream의 변경 내역과 선택할 커밋을 확인합니다. 자동으로 최신 커밋을 덮어쓰지 않습니다.
2. 기존 스냅샷과 새 버전의 차이를 검토하고, 자체 수정이 있는지 확인합니다.
3. 별도 브랜치에서 원래 경로 구조와 라이선스를 유지해 교체합니다. 삭제된 파일이 남지 않게 파일 목록도 비교합니다.
4. `SUPERPOWERS_SOURCE.md`의 커밋, 버전, 날짜를 갱신합니다.
5. 분야별 가이드의 링크와 설명이 새 버전에도 맞는지 확인합니다.

`.superpowers-source/`는 갱신 작업용 로컬 복제본이며 Git에서 제외됩니다. 배포되는 원문은 `references/superpowers/` 하나입니다.
